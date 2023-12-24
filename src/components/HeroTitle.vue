<template>
    <div class="relative md:mb-16 ">
      <!-- Outline Text (on top) -->
      <div class="flex text-[5vw] md:text-[12vw] font-bold tomorrow relative z-10 text-[#E2C799]" >
        {{ title }}
      </div>
  
      <!-- Original Text (behind) -->
      <div class="flex text-[5vw] md:text-[12vw] font-bold tomorrow absolute -bottom-2 left-2  md:-bottom-12 md:left-10 z-0 text-outline">
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
  