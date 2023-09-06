<script>
import SocialSidebar from './components/SocialSidebar.vue' // Import SocialSidebar
export default {
  components: {
    SocialSidebar
  }
}
</script>
<template>
  <div id="app">
    <div class="header">
      <div class="block"><router-link to="/">Home</router-link></div>
      <div class="block"><router-link to="/about">About</router-link></div>
      <div class="block"><router-link to="/contact">Contact</router-link></div>
    </div>

    <router-view />
    <SocialSidebar />
  </div>
</template>

<style>
.header {
  display: flex;
  justify-content: space-around;
  align-items: center;
  background-color: #f1f1f1;
  padding: 10px;
}

.block {
  padding: 10px;
}

.block:hover {
  background-color: #ddd;
}
a {
  color: #000;
  text-decoration: none;
}
</style>
