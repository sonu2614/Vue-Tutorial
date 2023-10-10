<template>
<h1 v-on:mousemove="getConsole()">Home Component</h1>
<h1>Email : {{ email }}</h1>
<h1>Mobile : {{ Mobile }}</h1>
<h1>Mobile : {{ Mobile=456 }}</h1>
<h1>Name : {{ getName() }}</h1>
<h1>SirName : {{ getSirName("Choudhary") }}</h1>
<!-- <h1>Data : {{ getData("100000") }}</h1> -->
<h1>All data : {{ getData().emailPassword }}</h1>
<button v-on:click="test()">Click Me 1</button>
<button v-on:click="getButton('Button 2 clicked')">Click Me 2</button>
<button v-on:dblclick="getButton('Button Doubled Clicked')">Button DoubledCliked</button>
<button v-on:click="increase()">Increase</button>
<h2>{{ count }}</h2>



</template>

<script>

export default {
    name: "Home",
    data() {
        return {
            count: 0,
            email: 'sonu@gmail.com',
            Mobile: '777777777',
            getName: function () {
                return "sonu kumar"
            },
        }
    },
    methods: {
        increase() {
            this.count = this.count + 1;
        },
        test() {
            alert("Function Called")
        },
        getButton(data) {
            alert(data)
        },
        getSirName(name) {
            return name;
        },
        getData() {
            return {
                firstName: 'sonu',
                emailPassword: '123'
            }
        },
        getConsole() {
            console.warn("Function calling")
        },
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
