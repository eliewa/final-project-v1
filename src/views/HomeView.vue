<script setup>
import AppCardVue from "../components/AppCard.vue";
import AppHeaderVue from "../components/AppHeader.vue";
</script>

<template>
  <AppHeaderVue text="Eli is happy"/>
  <div class="hero text-lg leading-6 text-white">
    <section class="ad h-screen w-full bg-cover bg-center text-3xl">
      <div class="flex-col banner mx-auto w-1/3 pt-44">
        <h1 class="text-5xl font-bold text-yellow-500">Welcome.</h1>
        <h1 class="hidden md:inline-block">
          Millions of movies, TV shows and people to discover.
        </h1>
        <h1>Explore now.</h1>
        <div class="search-bar mt-10 w-72 flex-col md:w-96">
          <label for="search" class="pr-10 pt-10">Search</label>
          <input
            type="text"
            id="search"
            class="block w-full border border-gray-300 bg-gray-50 p-2.5 text-sm text-gray-900 focus:border-blue-500 focus:ring-blue-500 dark:border-gray-600 dark:bg-gray-700 dark:text-white dark:placeholder-gray-400 dark:focus:border-blue-500 dark:focus:ring-blue-500"
            placeholder="Andor"
            required
          />
          <div class="flex justify-around overflow-y-scroll bg-black lg:p-7">
            <img src="../assets/images/andor.jpg" class="w-28" alt="" />
            <div class="title flex-col">
              <h2 class="text-md">Andor</h2>
              <p class="mt-5 text-sm text-gray-400">2022</p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>

  <main>
    <section class="border-b-2">
      <h1 class="text-4xl font-bold font-serif mt-10 pl-5">What's Popular</h1>
      <div class="gallery flex-wrap flex justify-center mx-auto mt-10">
      <AppCardVue
        text="Titanic"
        date="1997"
        image="src/assets/images/titanic.jpg"
      />
      <AppCardVue
        text="Andor"
        date="2022"
        image="src/assets/images/andor.jpg"
      />
      <AppCardVue
        text="Avatar"
        date="2004"
        image="src/assets/images/avatar.jpg"
      />
      <AppCardVue
        text="Batman"
        date="2022"
        image="src/assets/images/batman.jpg"
      />
      <AppCardVue />
      <AppCardVue />
      <AppCardVue />
      <AppCardVue />
     </div>
    </section>

    <section class="border-b-2">
      <h1 class="text-4xl font-bold font-serif mt-10 pl-5">Free to Watch</h1>
      <div class="gallery flex-wrap flex justify-center mx-auto mt-10">
      <AppCardVue
        text="Titanic"
        date="1997"
        image="src/assets/images/titanic.jpg"
      />
      <AppCardVue
        text="Andor"
        date="2022"
        image="src/assets/images/andor.jpg"
      />
      <AppCardVue
        text="Avatar"
        date="2004"
        image="src/assets/images/avatar.jpg"
      />
      <AppCardVue
        text="Batman"
        date="2022"
        image="src/assets/images/batman.jpg"
      />
      <AppCardVue />
      <AppCardVue />
      <AppCardVue />
      <AppCardVue />
     </div>
    </section>
    
  </main>
</template>

<style>
/* main {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
} */

.ad {
  background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
    url("../assets/images/andor.jpg");
}
</style>
