<template>
    <div>
        <h1>fetch data from API | AXIOS</h1>

        <h1>Employee List</h1>
        <div>
            <table>
                <tr>
                    <td>Name</td>
                    <td>Salary</td>
                    <td>Age</td>
                </tr>
                <tr v-for="item in list" :key="item.id">
                    <td>{{item.employee_name}}</td>
                    <td>{{item.employee_salary}}</td>
                    <td>{{item.employee_age}}</td>
                </tr>
            </table>
        </div>
    </div>
</template>

<script>

// importing package for api
//import Vue from 'vue';
//import VueAxios from 'vue-axios';
import axios from 'axios';
//Vue.use(VueAxios, axios);
//window.Vue = Vue;

export default {
    name:"Home15",
    data(){
        return{
            list:undefined
        }
    },
    mounted(){
        axios.get('https://dummy.restapiexample.com/api/v1/employees')
        .then(resp=>{
            this.list=resp.data.data
            //console.warn(resp.data.data)
        })
    }
}
</script>