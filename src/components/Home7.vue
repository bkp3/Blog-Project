<template>
    <div>
        <h1>Send props child to parent</h1>

        <button v-on:click="updateTitle">Update Parent Title</button>
    </div>
</template>
<script>
export default {
    name:'Home7',
    methods:{
        updateTitle(){
            //console.warn('Hello from title')
            this.$emit('changeTitle','Parent Updated')
        }
    }
}
</script>