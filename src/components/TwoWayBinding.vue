<template>
    <h1>Two Way Binding</h1>
    <input type="text" v-model="print"/>
    <h2>{{ print }}</h2>
  </template>
  
  <script>
  export default {
    name:"TwoWay",
    data(){
        return{
            print: " "
        }
    }
    
  }
  </script>
  
  <style>
</style>