<template>
    <h1>CheckBox</h1>
    <h3>Technology</h3>

    <label for="java">Java</label>
    <input type="checkbox" value="java" id="java" v-model="technology"/>

    <label for="html">HTML</label>
    <input type="checkbox" value="html" id="html" v-model="technology"/>

    <label for="css">CSS</label>
    <input type="checkbox" value="css" id="css" v-model="technology"/>

    <h4>Selected Technology : {{ technology }}</h4>
</template>

<script>
export default {
    name:"CheckBox",
    data()
    {
        return {
            technology:[]
        }
    }
}

</script>

<style>

</style>