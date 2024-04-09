<template>
  <div id="app">
    <contenu></contenu>
  </div>
  <RouterView />
</template>



<script>
import { RouterLink, RouterView } from 'vue-router'
import Contenu from './components/Contenu.vue';

export default {
  name: 'App',
  components: {
    'contenu': Contenu
      }
  }
</script>



<style scoped>

</style>
