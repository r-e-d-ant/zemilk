<template>
<div>
  <Header v-show="$route.name !== 'NotFound' "/>
  <router-view/>
  <Footer v-show="$route.name !== 'NotFound' "/>
</div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'

export default {
  components: {
    Header,
    Footer
  }
}
</script>

<style>
@import './assets/style.css';

</style>
