<script setup>

defineProps ({
    text: {
      default: "Andor",
      type: String,
    },
  })
</script>
<template>
  
  <div class="about">
    <h1>{{text}}</h1>
  </div>
</template>