<template>
    <div>
        <h1>props in vue js</h1>
        <!-- <h1>{{name}}</h1> -->

        <h1 v-for="user in users" :key="user.name">
            {{user.name}} --> {{user.email}}
        </h1>
    </div>
</template>
<script>
export default {
    name:'Home6',
    props:['users']
}
</script>