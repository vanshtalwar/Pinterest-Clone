<script setup>
import LeftBar from './components/LeftBar.vue';
import TopBar from './components/TopBar.vue';
import Gallery from './components/Gallery.vue';
</script>

<template>

  <div class=" flex h-screen w-full">

    <LeftBar/>

    <div class="content flex-1 mr-4">
      <TopBar />
      <Gallery />
    </div>

  </div>

</template>
