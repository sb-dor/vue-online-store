<script setup>
const props = defineProps({
  title: String,
  price: Number,
  isAdded: Boolean
})
</script>

<template>
  <div class="product">
    <h2>Товар: {{ props.title ?? '-' }}</h2>
    <h3>Цена: {{ props.price ?? '' }}</h3>
    <h4>Статус: {{ props.isAdded ? 'Добавлен' : 'Добавить' }}</h4>

    <!-- slot is needed if you want to write some additional code when you will use this component -->
    <slot></slot>
  </div>
</template>

<style scoped>
.product {
  border: 1px solid blue;
  padding: 10px;
  margin-bottom: 10px;
}
</style>
