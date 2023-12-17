<script setup>
const props = defineProps({
  imageUrl: String,
  title: String,
  price: Number,
  isInFavorite: Boolean,
  isAdded: Boolean,
  onAddToFavorite: Function,
  onAdd: Function
})
</script>

<template>
  <div
    class="flex-col border rounded-3xl p-4 w-max m-5 relative transition hover:shadow-xl hover:-translate-y-1"
  >
    <img
      @click="props.onAddToFavorite"
      :src="props.isInFavorite ? '/like-2.svg' : '/like-1.svg'"
      alt="Like"
      class="absolute top-5 left-5 cursor-pointer border rounded-lg"
    />
    <img :src="props.imageUrl" alt="image" class="w-60" />
    <p class="font-semibold text-base">{{ title ?? '-' }}</p>
    <div class="flex items-center justify-between mt-5">
      <div class="flex-col">
        <p class="text-slate-300 font-bold text-sm">Цена:</p>
        <p class="font-bold">{{ price ?? '-' }}р</p>
      </div>
      <img
        @click="props.onAdd"
        :src="isAdded ? '/checked.svg' : '/plus.svg'"
        alt="Plus"
        class="border rounded-lg cursor-pointer"
      />
    </div>
  </div>
</template>
