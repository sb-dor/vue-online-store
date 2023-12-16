<!--  in order to show another components add "setup" in "script" -->
<script setup>
import MyHello from './components/MyHello.vue'
import SendDataFromParent from '@/components/SendDataFromParent.vue'
</script>

<template>
  <!-- <h1>Flutter Developer!</h1>
  <h1>Going to write on vue</h1>
  <MyHello /> -->
  <p></p>
  <SendDataFromParent title="Кроссовки Puma" :price="9500" :is-added="true">
    <button class="temp_button_style">Добавить</button>
  </SendDataFromParent>
  <p></p>
  <SendDataFromParent title="Кроссовки Nike" :price="9500" :is-added="true" />
</template>

<style scoped>
.temp_button_style {
  background: green;
  border: none;
  padding: 10px;
  color: white;
  border-radius: 10px;
}
</style>
