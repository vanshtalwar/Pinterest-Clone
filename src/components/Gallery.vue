<script setup>
import GalleryItem from './GalleryItem.vue';

const items = [
  {
    id: 1,
    media: "/Pinterest-Clone/pins/pin1.jpeg",
    width: 1260,
    height: 1000,
  },
  {
    id: 2,
    media: "/Pinterest-Clone/pins/pin2.jpeg",
    width: 1260,
    height: 1400,
  },
  {
    id: 3,
    media: "/Pinterest-Clone/pins/pin3.jpeg",
    width: 1260,
    height: 1400,
  },
  {
    id: 4,
    media: "/Pinterest-Clone/pins/pin4.jpeg",
    width: 1260,
    height: 1000,
  },
  {
    id: 5,
    media: "/Pinterest-Clone/pins/pin5.jpeg",
    width: 1260,
    height: 1243,
  },
  {
    id: 6,
    media: "/Pinterest-Clone/pins/pin6.jpeg",
    width: 1260,
    height: 1568,
  },
  {
    id: 7,
    media: "/Pinterest-Clone/pins/pin7.jpeg",
    width: 1260,
    height: 1234,
  },
  {
    id: 8,
    media: "/Pinterest-Clone/pins/pin8.jpeg",
    width: 1260,
    height: 1400,
  },
  {
    id: 9,
    media: "/Pinterest-Clone/pins/pin9.jpeg",
    width: 1260,
    height: 1000,
  },
  {
    id: 10,
    media: "/Pinterest-Clone/pins/pin10.jpeg",
    width: 1260,
    height: 1000,
  },
  {
    id: 11,
    media: "/Pinterest-Clone/pins/pin11.jpeg",
    width: 1260,
    height: 1000,
  },
  {
    id: 12,
    media: "/Pinterest-Clone/pins/pin12.jpeg",
    width: 1260,
    height: 1400,
  },
  {
    id: 13,
    media: "/Pinterest-Clone/pins/pin13.jpeg",
    width: 1260,
    height: 1400,
  },
  {
    id: 14,
    media: "/Pinterest-Clone/pins/pin14.jpeg",
    width: 1260,
    height: 1600,
  },
  {
    id: 15,
    media: "/Pinterest-Clone/pins/pin15.jpeg",
    width: 1260,
    height: 1000,
  },
  {
    id: 16,
    media: "/Pinterest-Clone/pins/pin16.jpeg",
    width: 1260,
    height: 1260,
  },
  {
    id: 17,
    media: "/Pinterest-Clone/pins/pin17.jpeg",
    width: 1260,
    height: 1000,
  },
  {
    id: 18,
    media: "/Pinterest-Clone/pins/pin18.jpeg",
    width: 1260,
    height: 1260,
  },
  {
    id: 19,
    media: "/Pinterest-Clone/pins/pin19.jpeg",
    width: 1260,
    height: 1400,
  },
  {
    id: 20,
    media: "/Pinterest-Clone/pins/pin20.jpeg",
    width: 1260,
    height: 1260,
  },
  {
    id: 21,
    media: "/Pinterest-Clone/pins/pin21.jpeg",
    width: 1260,
    height: 1400,
  },
  {
    id: 22,
    media: "/Pinterest-Clone/pins/pin22.jpeg",
    width: 1260,
    height: 1890,
  },
  {
    id: 23,
    media: "/Pinterest-Clone/pins/pin23.jpeg",
    width: 1260,
    height: 1260,
  },
  {
    id: 24,
    media: "/Pinterest-Clone/pins/pin24.jpeg",
    width: 1260,
    height: 1260,
  },
  {
    id: 25,
    media: "/Pinterest-Clone/pins/pin25.jpeg",
    width: 1260,
    height: 1260,
  },
  {
    id: 26,
    media: "/Pinterest-Clone/pins/pin26.jpeg",
    width: 1260,
    height: 1260,
  },
  {
    id: 27,
    media: "/Pinterest-Clone/pins/pin27.jpeg",
    width: 1260,
    height: 1260,
  },
];
</script>

<template>
  <div class="grid grid-cols-2 lg:grid-cols-7 gap-4 w-full">
    <GalleryItem v-for="item in items" :key="item.id" :item="item" />
  </div>
</template>
