<template>
  <div id="app">
   <mt-button @click.native="handleClick">按钮</mt-button>

  </div>
</template>

<script>
export default {
  el: '#app',
  methods: {
    handleClick:function(){
      this.$toast('Hello world!');
    }
  }
}
</script>

<style>

</style>
