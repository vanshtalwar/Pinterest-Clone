<script setup>
import { ref } from "vue";

const currentUser = true; // change true/false to test

const showMenu = ref(false);
const toggleMenu = () => {
  showMenu.value = !showMenu.value;
};
</script>

<template>
  <!-- If user is logged in -->
  <div v-if="currentUser" class="relative inline-block text-center">
    <!-- Avatar + Arrow -->
    <div
      @click="toggleMenu"
      class="flex justify-center items-center gap-2 lg:mr-6 cursor-pointer"
    >
      <img
        class="h-8 rounded-full"
        src="/public/general/noAvatar.png"
        alt="avatar"
      />
      <img src="/public/general/arrow.svg" alt="arrow" />
    </div>

    <!-- Dropdown Menu (for logged in users) -->
    <div
      v-if="showMenu"
      class="absolute right-0 mt-2 w-28 rounded-2xl shadow-lg bg-white border p-2 z-10"
    >
      <ul class="flex flex-col gap-2 text-gray-700">
        <li class="px-3 py-2 hover:bg-gray-100 rounded-lg cursor-pointer">
          Profile
        </li>
        <li class="px-3 py-2 hover:bg-gray-100 rounded-lg cursor-pointer">
          Settings
        </li>
        <li class="px-3 py-2 hover:bg-gray-100 rounded-lg cursor-pointer">
          Logout
        </li>
      </ul>
    </div>
  </div>

  <!-- If no user is logged in -->
  <div v-else class="relative inline-block text-center">
    <!-- Login / Signup button -->
    <div
      @click="toggleMenu"
      class="text-xs m-0 p-0 hover:bg-gray-100 rounded-md lg:text-[15px] lg:p-2 cursor-pointer"
    >
      Login / Signup
    </div>

    <!-- Dropdown Menu (for guests) -->
    <div
      v-if="showMenu"
      class="absolute right-0 mt-2 w-28 rounded-2xl shadow-lg bg-white border p-2 z-10"
    >
      <ul class="flex flex-col gap-2 text-gray-700">
        <li class="px-3 py-2 hover:bg-gray-100 rounded-lg cursor-pointer">
          Login
        </li>
        <li class="px-3 py-2 hover:bg-gray-100 rounded-lg cursor-pointer">
          Signup
        </li>
      </ul>
    </div>
  </div>
</template>
