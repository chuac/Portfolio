<template>
    <div class="columns is-centered">
        <div class="column is-two-thirds">
            <header-nav></header-nav>
            <biography></biography>
        </div>
    </div>
</template>

<script>
import Header from './components/Header.vue'
import Biography from './components/Biography.vue'

export default {
  name: 'App',
  components: {
      'header-nav': Header,
      'biography': Biography
  }
}
</script>

<style>
#app {
  font-family: Camphor,Open Sans,Segoe UI,sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
