<template>
	<view class="edition">
		<view class="editionImage text-center">
			<image class="login__logo" src="../../static/logo.png" mode="aspectFit"></image>
			<view class="logo_font font-bold">LCP</view>
			<view class="logo_edition">版本:1.0.0 ></view>
		</view>
		<view class="editionBefore">
			<u-button text="已是最新版本"  size="small" shape="circle" color="#bbbbbb" disabled></u-button>
		</view>
		<view class="editionNew">
			<u-button text="有新的版本"  size="small" shape="circle" type="primary"></u-button>
		</view>
	</view>
</template>

<script>
</script>

<style lang="scss">
	.edition {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		.editionImage {
			position: relative;
			.login__logo {
				margin-top: 40px;
			}
			.logo_font {
				font-size: 20px;
				letter-spacing: 1px;
			}
			.logo_edition {
				color: #7d8ea8;
				letter-spacing: 1px;
			}
		}
		.editionBefore {
			width: 80%;
			margin-top: 100px;
		}
		.editionNew{
			width: 80%;
			margin-top: 15px;
		}
	}
</style>