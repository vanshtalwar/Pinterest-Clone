<script setup>
defineProps({
  item: {
    type: Object
  }
})
const getImageUrl = (path) => {
    return new URL(`../../public/pins/${path}`, import.meta.url).href;
};
</script>

<template>
  <div class="w-[90%]">
    <img :src="getImageUrl(item.media)" class="rounded-lg m-4 w-full h-auto"/>
  </div>
</template>

