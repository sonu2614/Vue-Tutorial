<template>
    <h1>For Loops</h1>
    <ul>
        <li v-for="item in technology" :key="item">
            {{ item }}
        </li>
    </ul>
    <br />
    <br />
    <ul>
        <li v-for="item in user" :key="item.email">
        Name is : {{ item.name }} and Email is : {{ item.email }} and Mobile number is :{{ item.mobile }}</li>
    </ul>
</template>

<script>
export default {
    name:"ForLoop",
    data(){
        return{
            technology:['java','php','css','html'],
            user:[{
                name:"Sonu",
                email:"sonu@gmail.com",
                mobile:745,
            },
            {
                name:"Ronit",
                email:"Ronit@gmail.com",
                mobile:745,
                

            },
        ]
        }
    }
}

</script>

<style>
li{
    color: red;
}
</style>