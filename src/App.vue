<script setup>
import { ref } from 'vue';
import { createRouter, createWebHashHistory } from 'vue-router';
import router from './router';
import HelloWorld from './components/HelloWorld.vue'

</script>

<template>
 <div class="nav">
    <router-link to="/">Home</router-link>
    |
    <router-link to="/about">About</router-link>
  </div>
  <router-view msg="Vite + Vue"></router-view>

</template>

<style scoped>
.nav{
  position: absolute;
  top: 20px;
  left: 20px;
}
</style>
