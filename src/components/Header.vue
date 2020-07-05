<template>
  <div class="Header">
      <Intro />
      <Menu />
  </div>
</template>

<script>
import Menu from './Menu.vue';
import Intro from './Intro.vue';

export default {
    name: 'Header',
    components: {
        Menu,
        Intro
    },
    
}
</script>

<style>
.Header {
    position: fixed;
    top: 0;
    right: 0;
    width: 100vw;
    display: flex;
    background-color: rgba(0,0,0,0.1);
    backdrop-filter: blur(10px);
}
</style>