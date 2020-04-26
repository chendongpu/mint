<template>
  <div id="index">
    我是main
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
    import { Toast } from 'mint-ui';
    export default {
        name: 'Toast',
        data(){
            return {
                examplename: "Toast"
            }
        },
        mounted(){

        },
        methods:{
            ToastA(){
                Toast('默认Toast');
            },
            ToastB(){
                Toast({
                    message: '操作成功',
                    iconClass: 'fa fa-check fa-2x'
                });
            },
            ToastC(){
                Toast({
                    message: '自定义位置',
                    position: 'bottom',
                    duration: 5000
                });
            }
        }
    }
</script>
<style scoped>
  ul {
    padding-left: 10px;
    padding-top: 20px;
    padding-right: 10px;
  }
  li {
    margin: 20px 0;
    list-style: none;
  }
</style>