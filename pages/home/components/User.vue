<template>
	<view class="bg-white mb-2 p-3" @click="onClick">
		<user-item :data="data" :avatarAuth="avatarAuth" :showId="showId" />
		<view class="mt-3">
			<u-swiper :list="data.imgList" :radius="0" :height="200" :autoplay="autoplay" indicator indicatorMode="dot"
				circular></u-swiper>
		</view>
	</view>
</template>

<script>
	export default {
		name: "LesUser",
		props: {
			data: Object,
			avatarAuth: {
				type: Boolean,
				default: false
			}, // 认证标识是否在头像上
			showId: {
				type: Boolean,
				default: false
			}, // 是否显示ID
			autoplay: {
				type: Boolean,
				default: false
			}, // 照片是否自动轮播
		},
		methods: {
			onClick() {
				this.$emit('click')
			}
		}
	}
</script>

<style lang="scss"></style>
