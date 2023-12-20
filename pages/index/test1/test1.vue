<template>
	<view>
		<button type="primary" @click="set1">设置标题1</button>
		<button type="primary" @click="set2">设置标题2</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			set1()
			{
				uni.setNavigationBarTitle({
					title:'标题1',
					success: () => {
						uni.showToast({
							title:'设置成功'
						})
					},
					fail: () => {
						uni.showToast({
							icon:'fail',
							title:'设置失败'
						})
					}
				})
			},
			set2()
			{
				uni.setNavigationBarTitle({
					title:'标题2',
					success: () => {
						uni.showToast({
							title:'设置成功'
						})
					},
					fail: () => {
						uni.showToast({
							icon:'fail',
							title:'设置失败'
						})
					}
				})
			},
			
		}
	}
</script>

<style>
button{
	margin: 5px;
}
</style>
