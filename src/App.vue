<template>
  <div id="app" class="container">
  <HeaderMenu></HeaderMenu>
    <div class="row">
      <div class="two columns">
        <ul>
          <li>Bio</li>
          <li>Bio</li>
          <li>Bio</li>
          <li>Bio</li>
          <li>Bio</li>
        </ul>
      </div>
      <div class="six columns">

      </div>
    </div>
  </div>
</template>

<script>
import HeaderMenu from './components/HeaderMenu.vue'

export default {
  name: 'App',
  components: {
    HeaderMenu
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
