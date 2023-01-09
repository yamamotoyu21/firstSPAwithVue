<script setup>
import { ref } from 'vue';
import { createRouter, createWebHashHistory } from 'vue-router';
import router from './router';
import HelloWorld from './components/HelloWorld.vue'
const id = ref('1');

</script>

<template>
 <div class="nav">
    <router-link to="/">Home</router-link>
    |
    <router-link to="/about">About</router-link>
    |
    <router-link to="`/user/${id}`">User</router-link>
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
