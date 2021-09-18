<template>
    <div>
        <h1>form validation</h1>
        
        <p v-if="error.length">
            <b>Please correct the following errors</b>
            <ul>
                <li v-for="e in error" :key="e.id">
                    {{e}}
                </li>
            </ul>
        </p>
        
        <form @submit="login">
            <input type="text" placeholder="enter your name" v-model="name"><br><br>
            <input type="password" placeholder="enter your password" v-model="password"><br><br>
            <button type="submit">Login</button>

        </form>
    </div>
</template>
<script>
export default {
    name:'Home11',
    data(){
        return{
            error:[],
            name:null,
            password:null
        }            
    },
    methods:{
        login(e){
            this.error=[];
            if(this.name && this.password){
                console.warn("no error");
            }
            if(!this.name){
                this.error.push("user name is required");
            }
            if(!this.password){
                this.error.push("password is required")
            }
            console.warn("Hello",this.error);
            e.preventDefault();
        }
    }
}
</script>