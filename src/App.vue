<template>
    <div class="columns is-centered is-mobile">
        <div class="column is-full-mobile is-four-fifths-tablet is-two-thirds-desktop is-two-thirds-widescreen is-two-thirds-fullhd">
            <header-nav></header-nav>
            <biography></biography>
            <projects></projects>
            <contact></contact>
            <br><br><br>
        </div>
    </div>
</template>

<script>
import Header from './components/Header.vue'
import Biography from './components/Biography.vue'
import Projects from './components/Projects.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  components: {
      'header-nav': Header,
      'biography': Biography,
      'projects': Projects,
      'contact': Contact
  }
}
</script>

<style>
/* #app {
  font-family: Camphor,Open Sans,Segoe UI,sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>
