<template>
  <div class="home  ">
  
  <Drawer/>
  <div class=" flex justify-center   mt-20 ">
    <div class="mx-1 md:mx-20 w-full  flex bg-black aspect-auto p-1 md:p-3  ">
      <hero/>
    </div>
   

  </div>

  </div>
</template>

<script>
// @ is an alias to /src
import Drawer from '@/components/Drawer.vue';
import Hero from '@/components/Hero.vue';
export default {
  name: 'HomeView',
  components: {
    Drawer,
    Hero
  }
}
</script>
