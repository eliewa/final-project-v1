<script setup>
import { stringifyExpression } from '@vue/compiler-core';
import { def } from '@vue/shared';


  defineProps ({
    text: {
      default: "Andor",
      type: String,
    },
    
    date: {
      default: 2022,
      type: Number,
    },
   
    image: {
      default: "src/assets/images/andor.jpg",
      type: String
    }
  })

</script>
<template>
  <main>
    <article class="w-52 h-auto pb-10 text-lg">
      <img v-bind:src="image" alt="" class="h-60 rounded-lg shadow-sm hover:shadow-xl">
      <h1 class="font-black">{{text}}</h1>
      <h1 class="font-light">{{date}}</h1>
      
    </article> 
  </main>
</template>