<template>
  <div class="home">
    <Navbar />
    <List />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Navbar from '../components/Navbar.vue';
import List from '../components/List.vue';

export default Vue.extend({
  name: 'home',
  components: {
    List,
    Navbar,
  },
});
</script>
