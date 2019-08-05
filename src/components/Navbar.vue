<template>
  <nav class="navbar">
    <div>
      <img alt="Vue logo" src="../assets/logo.png" width="200px">
    </div>
    <div class="title">
      <h2>Rede de Edtechs</h2>
    </div>
    <div class="sponsors">
      <p>Apoiadores: </p>
      <div>
        <a v-for="sponsor in sponsors" :key="sponsor.name" :href="sponsor.site" target="_blank">
          <img
            class="sponsor-logo"
            :src="require(`../assets/${sponsor.logo}`)"
            :alt="`${sponsor.name} logo`"
            height="50px">
        </a>
      </div>
    </div>
  </nav>
</template>

<script lang="ts">
import Vue from 'vue';
import sponsors from '../source/sponsors';

export default Vue.extend({
  computed: {
    sponsors: () => sponsors,
  },
});
</script>

<style lang="less" scoped>
.navbar {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  margin: 0 20px;
  padding-bottom: 10px;
  border-bottom: 1px solid rgba(0, 0, 0, 0.08);
}

.sponsors {
  min-width: 200px;
}

.sponsor-logo {
  margin: 0 10px;
}

.title {
  @media (max-width: 800px) { display: none; }
}
</style>
