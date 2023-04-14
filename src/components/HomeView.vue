

<template>
    <main>
        <button @click = "counter++">up</button>
        <h3>{{ counter }}</h3>
        <button @click = "counter--">down</button>
        <h3>{{ person.name }} {{ person.age }}</h3>
        <button @click="updatePerson">update person</button>
    </main>
</template>

<script setup lang="ts">

    import { reactive, ref } from "vue";
    const counter = ref(0)

    const person = reactive({name:"inzaky",age:47})

    const updatePerson = () => {
        person.name = "Ammar",
        person.age = 45

    }

</script>

<style scoped>

</style>