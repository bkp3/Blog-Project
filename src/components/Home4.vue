<template>
    <div>
        <h1 class="homestyle">Class and Style Bindings</h1>
        <h1 v-bind:style="{color:'blue'}">style binding</h1>
        <h1 v-bind:class="{display:show}">class binding with object</h1>
        <h1 v-bind:class="[aClass]">class binding with array</h1>
        <h1 v-bind:class="[show?'yesShow':'noShow']">class binding with condition</h1>

    </div>
</template>
<script>
export default {
    name:"Home4",
    data(){
        return{
            show:false,
            aClass:'arrayClass'
        }
    }

};
</script>
<style>
.homestyle{
    color: rgb(204, 29, 38)
}
.display{
    color: yellow;
}
.arrayClass{
    color: aqua;
}
</style>