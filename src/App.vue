<template>
  <div>
    <app-header></app-header>
    <app-body></app-body>
    <app-footer></app-footer>
  </div>
</template>

<script>
// Imports
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Body from './components/Body.vue';
export default {
  components: {
    'app-header': Header,
    'app-footer': Footer,
    'app-body': Body
  },
  data () {
    return {
    }
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
