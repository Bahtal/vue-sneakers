<script setup>
import Cart from './Cart.vue'
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
      image-url="/sneakers/sneakers-1.jpg"
      brend="Мужские Кроссовки Nike Blazer Mid Suede"
      :price="12999"
      :on-click-add="onClickAdd"
      :on-click-favorite="onClickFavorite"
    />
    <Cart
      image-url="/sneakers/sneakers-2.jpg"
      brend="Мужские Кроссовки Nike Air Max 270"
      :price="12999"
      :is-added="true"
      :is-favorited="true"
    />
    <Cart
      image-url="/sneakers/sneakers-3.jpg"
      brend="Мужские Кроссовки Nike Blazer Mid Suede"
      :price="8499"
    />
    <Cart
      image-url="/sneakers/sneakers-4.jpg"
      brend="Кроссовки Puma X Aka Boku Future Rider"
      :price="8999"
    />
    <Cart
      image-url="/sneakers/sneakers-5.jpg"
      brend="Мужские Кроссовки Under Armour Curry 8"
      :price="15199"
    />
    <Cart
      image-url="/sneakers/sneakers-6.jpg"
      brend="Мужские Кроссовки Nike Kyrie 7"
      :price="11299"
    />
    <Cart
      image-url="/sneakers/sneakers-7.jpg"
      brend="Мужские Кроссовки Jordan Air Jordan 11"
      :price="10799"
    />
    <Cart
      image-url="/sneakers/sneakers-8.jpg"
      brend="Мужские Кроссовки Nike LeBron XVIII"
      :price="16499"
    />
  </div>
</template>
