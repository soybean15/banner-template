<template>
  <div class="home   ">
  
  <Drawer/>
  <div class=" flex justify-center   ">
    <div class=" max-w-[1200px] flex bg-black aspect-video p-3  ">
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
