<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <router-view/>
  </div>
</template>

<style lang="less">
#app {
  // font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

@font-face {
  font-family: 'Comfortaa';
  src: url('./../public/fonts/Comfortaa/Comfortaa-Bold.ttf');
}

@font-face {
  font-family: 'Nunito';
  src: url('./../public/fonts/Nunito_Sans/NunitoSans-Light.ttf');
}

h1, h2, h3, h4, h5, h6, th {
  font-family: 'Comfortaa', cursive;
  color: #2c4877;
}

p, td {
  font-family: 'Nunito', sans-serif;
}
</style>
