<script setup>
import GalleryItem from './GalleryItem.vue';

import { ref } from 'vue'


const items = [
  {
    id: 1,
    media: "pin1.jpeg",
    width: 1260,
    height: 1000,
  },
  {
    id: 2,
    media: "pin2.jpeg",
    width: 1260,
    height: 1400,
  },
  {
    id: 3,
    media: "pin3.jpeg",
    width: 1260,
    height: 1400,
  },
  {
    id: 4,
    media: "pin4.jpeg",
    width: 1260,
    height: 1000,
  },
  {
    id: 5,
    media: "pin5.jpeg",
    width: 1260,
    height: 1243,
  },
  {
    id: 6,
    media: "pin6.jpeg",
    width: 1260,
    height: 1568,
  },
  {
    id: 7,
    media: "pin7.jpeg",
    width: 1260,
    height: 1234,
  },
  {
    id: 8,
    media: "pin8.jpeg",
    width: 1260,
    height: 1400,
  },
  {
    id: 9,
    media: "pin9.jpeg",
    width: 1260,
    height: 1000,
  },
  {
    id: 10,
    media: "pin10.jpeg",
    width: 1260,
    height: 1000,
  },
  {
    id: 11,
    media: "pin11.jpeg",
    width: 1260,
    height: 1000,
  },
  {
    id: 12,
    media: "pin12.jpeg",
    width: 1260,
    height: 1400,
  },
  {
    id: 13,
    media: "pin13.jpeg",
    width: 1260,
    height: 1400,
  },
  {
    id: 14,
    media: "pin14.jpeg",
    width: 1260,
    height: 1600,
  },
  {
    id: 15,
    media: "pin15.jpeg",
    width: 1260,
    height: 1000,
  },
  {
    id: 16,
    media: "pin16.jpeg",
    width: 1260,
    height: 1260,
  },
  {
    id: 17,
    media: "pin17.jpeg",
    width: 1260,
    height: 1000,
  },
  {
    id: 18,
    media: "pin18.jpeg",
    width: 1260,
    height: 1260,
  },
  {
    id: 19,
    media: "pin19.jpeg",
    width: 1260,
    height: 1400,
  },
  {
    id: 20,
    media: "pin20.jpeg",
    width: 1260,
    height: 1260,
  },
  {
    id: 21,
    media: "pin21.jpeg",
    width: 1260,
    height: 1400,
  },
  {
    id: 22,
    media: "pin22.jpeg",
    width: 1260,
    height: 1890,
  },
  {
    id: 23,
    media: "pin23.jpeg",
    width: 1260,
    height: 1260,
  },
  {
    id: 24,
    media: "pin24.jpeg",
    width: 1260,
    height: 1260,
  },
  {
    id: 25,
    media: "pin25.jpeg",
    width: 1260,
    height: 1260,
  },
   {
    id: 1,
    media: "pin1.jpeg",
    width: 1260,
    height: 1000,
  },
  {
    id: 2,
    media: "pin2.jpeg",
    width: 1260,
    height: 1400,
  },
  {
    id: 3,
    media: "pin3.jpeg",
    width: 1260,
    height: 1400,
  },
];
</script>

<template>
  <div class="grid grid-cols-2 lg:grid-cols-7 gap-4 w-full">
    <GalleryItem v-for="item in items" :key="item.id" :item="item" />
  </div>
</template>
