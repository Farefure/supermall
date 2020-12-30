<template>
  <div id="app">
    <router-view/>
    <main-tab-bar/>
  </div>
</template>

<script>
  import MainTabBar from 'components/content/mainTabBar/MainTabBar'
  export default {
   data() {
     return {
     }
   },
    name: 'App',
    components: {
      MainTabBar
    },
  }
</script>

<style>
  @import "assets/css/base.css";
</style>
