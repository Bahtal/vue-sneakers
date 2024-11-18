<script setup>
import CardItemList from './CardItemList.vue'
import DrawerHead from './DrawerHead.vue'
</script>
<template>
  <div>
    <div class="fixed top-0 left-0 h-full w-full bg-black z-10 opacity-70"></div>
    <div class="flex flex-col bg-white w-96 h-full fixed right-0 top-0 z-20 p-8">
      <div class="flex-1">
        <DrawerHead />
        <CardItemList />
      </div>
      <div class="flex flex-col gap-4 mt-7">
        <div class="flex gap-2 items-center">
          <span>Итог:</span>
          <div class="flex-1 border-b border-dashed"></div>
          <b>12900 $</b>
        </div>
        <div class="flex gap-2 items-center">
          <span>Налог 5%:</span>
          <div class="flex-1 border-b border-dashed"></div>
          <b>900 $</b>
        </div>
        <button
          class="bg-lime-500 mt-4 w-full rounded-xl py-3 text-white transition disabled:bg-slate-300 hover:bg-lime-600 active:bg-lime-700 cursor-pointer relative"
        >
          Оформить заказ
          <img class="absolute inset-y-1/2 -translate-y-1/2 right-7" src="/arrow-next.svg" alt="" />
        </button>
      </div>
    </div>
  </div>
</template>
