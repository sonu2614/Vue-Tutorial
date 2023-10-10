<template>
<h1>Radio</h1>
<h3>who</h3>

<label for="student">Student</label>
<input type="radio" value="student" id="student" v-model="who" name="who" />

<label for="coder">Coder</label>
<input type="radio" value="coder" id="coder" v-model="who" name="who" />

<label for="developer">Developer</label>
<input type="radio" value="developer" id="developer" v-model="who" name="who" />

<h4>I am a : {{ who }}</h4>
</template>

<script>
export default {
    name: "RadioBox",
    data() {
        return {
            who:null,
        }
    }
}
</script>

<style>

</style>
