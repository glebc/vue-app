<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/changelog">Change Log</router-link>
    </div>
    <router-view/>
  </div>
</template>

<script>
  export default {
    beforeCreate () {
      this.$Loading.start()
    },
    created () {
      this.$Loading.finish()
    }
  }
</script>

<style lang="scss">
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    h1 {
      margin: 0 0 20px;
      text-align: center;
    }
  }
  #nav {
    text-align: center;
    padding: 30px;
    a {
      font-weight: bold;
      color: #2c3e50;
      &.router-link-exact-active {
        color: #42b983;
      }
    }
  }
  .at-loading-bar.at-loading-bar--success {
    .at-loading-bar__inner {
      background-color: #42b983;
    }
  }
</style>
