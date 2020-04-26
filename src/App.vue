<template>
  <div id="app">
      <div class="content-div">
          <router-view/>
      </div>
      <footer-bar class="footer"></footer-bar>
  </div>
</template>

<script>
    import Footer from './components/FooterBar.vue'
export default {
  el: '#app',
    components: {
        'footer-bar': Footer
    },
}
</script>

<style>

</style>
