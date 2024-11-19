<script setup>
import Cart from './Cart.vue'

defineProps({
  items: Array,
})
const onClickAdd = () => {
  alert('Добавить')
}
const onClickFavorite = () => {
  alert('Нравится')
}
</script>
<template>
  <div class="grid grid-cols-4 gap-5">
    <Cart
      v-for="item in items"
      :key="item.id"
      :image-url="item.imageUrl"
      :title="item.title"
      :price="item.price"
      :on-click-add="onClickAdd"
      :on-click-favorite="onClickFavorite"
    />
  </div>
</template>
