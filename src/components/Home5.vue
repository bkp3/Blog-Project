<template>
    <div>
        <h1>Data Binding in vue JS</h1>
        <h1>{{message}}</h1>
        <input type="text" v-model="message">

        <h1 style="white-space:pre-line">{{messageMulti}}</h1>
        <textarea type="text" v-model="messageMulti"/>
    </div>
</template>
<script>
export default {
    name:'Home5',
    data(){
        return{
            message:'Hello Binding',
            messageMulti:'Hello Binding'
        }
    }
}
</script>