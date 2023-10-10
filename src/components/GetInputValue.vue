<template>
<h1>Get Input Value</h1>
<input type="email" placeholder="Enter Email" v-model="email"/>
<br/>
<br />
<input type="password" placeholder="Enter Password" v-model="password"/>
<br /><br />
<button v-on:click="getData()" type="button">Get Values</button>
</template>

  
<script>
export default {
    name: "GetInputValue",
    data(){
        return{
            email:null,
            password:null,
        }
    },
    methods:{
        getData()
        {
            console.warn("vALUES: ",this.email,this.password)
        }
    }

}
</script>

  
<style>
*{
    background-color: gray;
}
input{
    background-color: white;
}
button{
    background-color: skyblue;
    border-radius: 20px;
    padding: 10px;
}
</style>
