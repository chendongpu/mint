<template>
	<div id="index">

		<div v-for="item in nameList">
			<span>{{item.name}}</span>
			<span>{{item.nick}}</span>
		</div>
		我的界面
	</div>
</template>
<style scoped>
	#index {
		display: flex;
		justify-content: center;
		margin-top: 100px;
	}
</style>
<script>
	export default {
		data() {
                return {
                    nameList: []
			}
		},
		created() {
			   this.$http.get('/api/test.json').then((response) => {

				console.log(response.data)
				//响应正确回调
				this.nameList = response.data.first; //把数据存放到data中
			}).catch(err => {

               })
		}

	}
</script>