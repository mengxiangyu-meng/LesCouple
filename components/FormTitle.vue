<template>
	<view class="form-item d-flex align-center">
		<view>{{ title }}</view>
		<view v-if="description" class="form-item__desc">（{{ description }})</view>
	</view>
</template>

<script>
	export default {
		name: "FormTitle",
		props: {
			title: String,
			description: String,
		},
	}
</script>

<style lang="scss">
	.form-item__desc {
		color: $uni-text-color-grey;
		font-size: 12px;
	}
</style>
