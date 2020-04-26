<template>
  <div id="index">
    这里是应用中心
    <mt-button size="large" @click="go">测试跳转</mt-button>
  </div>
</template>
<style scoped>
  #index{
    display: flex;
    justify-content: center;
    margin-top: 100px;
  }
</style>
<script>
  export default{
      methods: {
          go() {
              this.$router.push('/fa');//要跳转的界面
          }
      }
  }
</script>
