<template>
	<view class="content">
			<swiper3D 
			 :imgList="imgList" 
			:currentIndexParameter="currentpic"
			:delayTime="2"
			:turn="false"
			>
			</swiper3D>
	</view>
</template>

<script>
	import swiper3D from '../../components/swiper3D.vue';
	export default {
		data() {
			return {
				imgList: [
					{url: 'other?id=1' , src: '../../static/s0.png' },
					{url: '' , src: '../../static/s1.png' },
					{url: '' , src: '../../static/s2.png' },
					{url: '' , src: '../../static/s3.png' },
					{url: 'other?id=2' , src: '../../static/s4.png' },
				],
				currentpic:4
			}
		},
		onLoad() {
			setTimeout(()=>{
this.imgList=[
		{url: 'other?id=1' , src: '../../static/s3.png' },
		{url: '' , src: '../../static/s1.png' },
		{url: '' , src: '../../static/s4.png' },
		{url: '' , src: '../../static/s2.png' },
		{url: 'other?id=2' , src: '../../static/s1.png' },
	]
	console.log(this.imgList)
},2000)
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
