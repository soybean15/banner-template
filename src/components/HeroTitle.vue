<template>
    <div class="relative mb-16">
      <!-- Outline Text (on top) -->
      <div class="flex text-8xl font-bold tomorrow relative z-10 ">
        {{ title }}
      </div>
  
      <!-- Original Text (behind) -->
      <div class="flex text-8xl font-bold tomorrow absolute -bottom-12 left-10 text-red-400 z-0 text-outline">
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
    -webkit-text-stroke: 1px black; /* WebKit/Blink browsers */
    text-stroke: 1px black; /* Standard syntax */
    color: white; /* Text color */
  }
  </style>
  