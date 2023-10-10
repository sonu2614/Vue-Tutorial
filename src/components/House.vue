<template>
    <h1>Pass Data to child Component</h1>
    <Child />
</template>

<script>
import Child from './Child.vue';
export default {
    name:"HouseCom",
    components:{
        Child
    }
}
</script>