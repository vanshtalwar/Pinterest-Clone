
<script setup>
import UserButton from './UserButton.vue';


</script>

<template>
  <div class="flex justify-between items-center">

<div class="w-60 m-4 px-4 h-12 rounded-xl bg-gray-100 hover:bg-gray-200 flex items-center gap-4
 lg:w-330 ">
  <img class="h-4" src="/public/general/search.svg" alt="">
  <input class="focus:outline-hidden w-50 lg:w-320"  type="text" placeholder="Search">
</div>

<UserButton/>

  </div>
</template>

