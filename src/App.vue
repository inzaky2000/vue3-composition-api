//การเขียนแบบใหม่
<template>
  <!-- <h1>{{ title }}</h1>
  <h2>{{ description }}</h2>
  <h3>{{ year }}</h3> -->
  <HomeView />

</template>
<script setup lang="ts">
    // import { ref } from 'vue';
    import HomeView from './components/HomeView.vue';

    // const title = ref("Hello World")
    // const description = ref("How are you")
    // const year = ref(2023)
</script>

<style scoped>

</style>

//ข้างล่างเป็นการเขียนแบบเดิม
<!-- <template>
  <h1>{{ data.title }}</h1>
  <h2>{{ data.description }}</h2>
  <h3>{{ data.year }}</h3>
</template>

<script lang="ts">
import { defineComponent, ref,reactive } from 'vue'

export default defineComponent({
  // แบบใหม่ เป็น Composition api
  setup () {
    // const title = ref("Hello World")
    // const description = ref("How are you")
    // const year = ref(2023)
    // console.log(title)

    // Reactive จะรองรับฉบับ objects เท่านั้น
    const data = reactive ({
      title: "Hello World!",
      description: "welcome evevrybody",
      year: 2022
    })

    console.log(data)

    setTimeout(() => {
      // title.value = "Hello Inzaky"
      data.title = "Hello Peter"
    }, 2000)

    // return {title, description, year}
    return { data }
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

</style> -->