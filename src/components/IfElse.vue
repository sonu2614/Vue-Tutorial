<template>
<h1>If Else Condition</h1>

<h2 v-if="show">If Condition</h2>
<h2 v-else>Else Condition</h2>

<button v-on:click="show=!show">Toggle</button>
</template>

<script>
export default {
    name:"IfElse",
    data()
    {
        return{
            show:false
        }
    }
}

</script>

<style>
h2{
    color: orange;
}
</style>