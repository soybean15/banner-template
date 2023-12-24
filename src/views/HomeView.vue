<template>
  <div class="home  ">
  
  <Drawer/>
  <div class=" flex justify-center">
    <hero/>

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
