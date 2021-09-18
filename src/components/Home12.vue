<template>
    <div>
        <h1>beforecreate and created life cycle methods</h1>

        <h1>{{name}}</h1>
    </div>
</template>
<script>
export default {
    name:'Home12',
    data(){
        return{
            name:"Rakesh Kumar"
        }
    },
    beforeCreate(){
        this.name="sam"
        console.warn("beforeCreate",this.name);
    },
    created(){
        
        console.warn("created",this.name);
    }
}
</script>