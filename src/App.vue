<!--  in order to show another components add "setup" in "script" -->
<script setup>
import MyHello from './components/MyHello.vue'
import SendDataFromParent from '@/components/SendDataFromParent.vue'
import Header from './components/Header.vue'
import ListCards from '@/components/ListCards.vue'
import Drawer from '@/components/Drawer.vue'
</script>

<template>
  <!-- <h1>Flutter Developer!</h1>
  <h1>Going to write on vue</h1>
  <MyHello /> -->
  <!-- <p></p> -->
  <!-- <div class="mb-40 text-slate-500">
    <SendDataFromParent title="Кроссовки Puma" :price="9500" :is-added="true">
      <button class="temp_button_style">Добавить</button>
    </SendDataFromParent>
  </div> -->
  <!-- <SendDataFromParent title="Кроссовки Nike" :price="9500" :is-added="true" /> -->
  <Drawer />
  <div class="bg-white w-4/5 m-auto rounded shadow-xl mt-10">
    <Header />
    <div class="pl-8">
      <h1 class="font-bold text-2xl">Все кроссовки</h1>
    </div>
    <ListCards />
  </div>
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
