<script setup>
import Card from './Card.vue'
</script>

<template>
  <div class="grid grid-cols-4 gap-1">
    <Card
      imageUrl="/sneakers/sneakers-1.jpg"
      title="Мужские кроссовки nike"
      :price="5000"
      :isAdded="true"
      :isInFavorite="false"
    />
  </div>
</template>
