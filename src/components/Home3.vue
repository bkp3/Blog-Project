<template>
    <div>
        <h1>This is template</h1>
        <h1 v-once>{{name}}</h1>
        <h1>{{name}}</h1>
        <h1>{{a+b}}</h1>
        <button v-on:click="updateText">Click me</button>
        <h1>{{ok?"Yes":"No"}}</h1>
        <p v-html="rowHtml"></p>
        <button v-bind:disabled="disableBtn">Disable Button</button>
    </div>
</template>
<script>
export default {
    name:'Home3',
    data(){
        return{
            name:'Ramesh',
            a:10,
            b:122,
            ok:true,
            rowHtml:"<h1>Add HTML as property</h1>",
            disableBtn:false
        }
    },
    methods:{
        updateText(){
            this.ok=!this.ok
        }

    }
}
</script>