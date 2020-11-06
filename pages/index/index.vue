<template>
	<view class="content">
			<swiper3D  :imgList="imgList"></swiper3D>
	</view>
</template>

<script>
	import swiper3D from '../../components/swiper3D.vue';
	export default {
		data() {
			return {
				imgList: [
					{url: 'other?id=1' , src: '../../static/winbox.png' },
					{url: '' , src: '../../static/winbox.png' },
					{url: '' , src: '../../static/winbox.png' },
					{url: '' , src: '../../static/winbox.png' },
					{url: 'other?id=2' , src: '../../static/winbox.png' },
				],
			}
		},
		onLoad() {

		},
		methods: {

		},
		components: {
			swiper3D
		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
