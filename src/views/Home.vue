<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" width="300px">
    <List />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import List from '../components/List.vue';

export default Vue.extend({
  name: 'home',
  components: {
    List,
  },
});
</script>
