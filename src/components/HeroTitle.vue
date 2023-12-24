<template>
    <div class="relative mb-16 ">
      <!-- Outline Text (on top) -->
      <div class="flex text-8xl font-bold tomorrow relative z-10 text-[#E2C799]" >
        {{ title }}
      </div>
  
      <!-- Original Text (behind) -->
      <div class="flex text-8xl font-bold tomorrow absolute -bottom-12 left-10 z-0 text-outline">
        {{ title }}
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: ['title'],
  };
  </script>
  
  <style>
  .text-outline {
    -webkit-text-stroke: 2px #E2C799;
    text-stroke: 2px #E2C799;
    color: black; /* Text color */
  }
  </style>
  