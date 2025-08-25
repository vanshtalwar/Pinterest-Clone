<script setup>
defineProps({
  item: {
    type: Object
  }
})
</script>

<template>
  <div class="w-[90%]">
    <img :src="item.media" class="rounded-lg m-4 w-full h-auto"/>
  </div>
</template>

