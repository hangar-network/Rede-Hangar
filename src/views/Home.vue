<template>
  <div class="home">
    <Navbar />
    <div class="last-modified">
      <p class="last-modified__text">Última modificação em: 04 de Agosto de 2019</p>
    </div>
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

<style lang="less" scoped>
.last-modified {
  width: 100%;

  &__text {
    float: left;
    float: right;
    font-size: 13px;
    margin: 10px 40px 0 0;
  }
}
</style>
