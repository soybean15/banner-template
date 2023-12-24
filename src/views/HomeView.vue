<template>
  <div class="home  ">
  
  <Drawer/>
  <div class=" flex justify-center   mt-20 ">
    <div class="max-w-[1100px] md:max-w-[1400px] flex bg-black aspect-video p-1 md:p-3  ">
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
