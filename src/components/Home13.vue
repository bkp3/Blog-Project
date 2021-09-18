<template>
    <div>
        <h1> beforeMount and Mounted life cycle methods</h1>
        <h1>{{name}}</h1>

    </div>
</template>
<script>
export default {
    name:"Home13",
    data(){
        return{
            name:"Mukesh Kumar"
        }
    },
    beforeMount(){
        console.log("beforeMount",this.$el);
    },
    mounted(){
        console.log("mounted",this.$el);
    }
}
</script>