<template>
  <h1>{{ title }}</h1>
  <h2>{{ description }}</h2>
  <h3>{{ year }}</h3>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'

export default defineComponent({
  // แบบใหม่ เป็น Composition api
  setup () {
    const title = ref("Hello World")
    const description = ref("How are you")
    const year = ref(2023)

    console.log(title)

    setTimeout(() => {
      title.value = "Hello Inzaky"
    }, 2000)

    return {title, description, year}
  },

  // แบบเดิม เป็น Option api
  // data(){
  //   return {
  //     title: "Hello World"
  //   }
  // },

  // mounted() {
  //   setTimeout(() => {
  //     this.title = "Hello Inzaky"
  //   }, 2000);
  // },
})
</script>

<style scoped>

</style>