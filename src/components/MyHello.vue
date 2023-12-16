<!-- options api -->
<script>
export default {
  data() {
    return {
      count: 0
    }
  },
  methods: {
    increment() {
      this.count++
    }
  }
}
</script>

<!-- compositions api -->
<script setup>
import { ref } from 'vue'
let countCompositionApi = ref(0)

function incrementCompositionApi() {
  countCompositionApi.value++
}

function updateCount(event) {
  countCompositionApi.value = Number(event.target.value)
}
</script>

<template>
  <h1>{{ countCompositionApi }}</h1>
  <button @click="incrementCompositionApi">+</button>
  <input @keyup.enter="updateCount" />
</template>

<!-- "scoped" means you write styles only in for this "templete" and every class for css will work only for this templete-->
<style scoped>
body {
  background: red;
}
</style>
