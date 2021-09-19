<template>
    <div>
        <h1>beforeDestroy and destroyed life cycle methods</h1>
        <h1>{{name}}</h1>


    </div>
</template>
<script>
export default {
    name:'Home14',
    data(){
        return{
            name:"Home Component"
        }
    },
    // beforeDestroy(){
    //     console.warn("before destroy")
    // },
    // destroyed(){
    //     console.warn("destroyed")
    // }
}
</script>