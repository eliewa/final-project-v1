<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header class="hero text-lg leading-6 text-white">
    <nav class="flex justify-between bg-gray-900">
      <span class="fa-solid fa-bars p-5 text-4xl md:invisible"></span>
      <div class="top-7 m-auto md:absolute">
        <span class="p-5 font-serif text-2xl"
          >Film <span class="font-serif text-yellow-500">Junkies.</span></span
        >
      </div>

      <div class="nav-links m-auto">
        <ul class="hidden justify-between md:flex">
          <li class="pr-10 pt-5 hover:text-yellow-500"><RouterLink to="/">Movies</RouterLink></li>
          <li class="pr-10 pt-5 hover:text-yellow-500">TV Shows</li>
          <li class="pr-10 pt-5 hover:text-yellow-500"><RouterLink to="/about">About</RouterLink></li>
          <li class="pt-5 hover:text-yellow-500">API</li>
        </ul>
      </div>
      <div class="login p-5 mt-3 mr-5 self-center">
        <span class="pr-5 hover:text-yellow-500">Login</span>
        <i class="fa-regular fa-user invisible md:visible"></i>
        <!-- <span class="md:hidden">Join the Team</span> -->
      </div>
    </nav>
    <nav>
    </nav>
  </header>

  <RouterView />
</template>
