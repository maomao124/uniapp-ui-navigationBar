<template>
	<view>
		<button type="primary" @click="set1">showNavigationBarLoading</button>
		<button type="primary" @click="set2">hideNavigationBarLoading</button>
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
				uni.showNavigationBarLoading({});
			},
			set2()
			{
				uni.hideNavigationBarLoading();
			},
		},
		onReady: () => {
			uni.setNavigationBarTitle({
				title:'标题'
			})
		}
	}
</script>

<style>
button{
	margin: 5px;
}
</style>
