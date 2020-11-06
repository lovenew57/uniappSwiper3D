# uniappSwiper3D
一个开源的Uniapp的3d轮播组件


重要参数说明：

		imgList : 一个数组，存放轮播图片的地址 
    特别说明：如果有跳转的话，这里的元素个数一定要和imgUrl的一致 而且内部的参数名一定是src
    例子：
    				imgList: [
              { src: '../../static/winbox1.png' },
              { src: '../../static/winbox2.png' },
              { src: '../../static/winbox3.png' },
              { src: '../../static/winbox4.png' },
              { src: '../../static/winbox5.png' },
              { src: '../../static/winbox6.png' },
				    ]


		imgUrl : 一个数组，轮播图片跳转对应的地址
    特别说明：这里的元素个数一定要和imgList的一致 而且内部的参数名一定是url
    例子：				
        imgUrl: [
              { url: 'other' },
              { url: 'other' },
              { url: 'other' },
              { url: 'other' },
              { url: 'other' },
              { url: 'other' }
            ],
    
    haveUrl : { type : Boolean, default : true },//是否进行页面的跳转
    特别说明：默认是true 如果不进行跳转 不传imgUrl或者直接设置fales也可以
    
    
    
		currentIndexParameter  : {type : Number, default : 1},//默认放在中间的图片
		movewidthParameter  : {type : Number, default : 0.4},//图片位移
		openTypeParameter  :{type : String, default : "navigate"},//switchTab 也是是去tabbar页面 普通页面为navigate 


使用例子：
<template>
	<view class="content">
			<swiper3D  :imgList="imgList" :imgUrl="imgUrl"></swiper3D>
	</view>
</template>

<script>
	import swiper3D from '../../components/swiper3D.vue';
	export default {
		data() {
			return {
				imgList: [
					{ src: '../../static/winbox.png' },
					{ src: '../../static/winbox.png' },
					{ src: '../../static/winbox.png' },
					{ src: '../../static/winbox.png' },
					{ src: '../../static/winbox.png' },
					{ src: '../../static/winbox.png' },
				],
				imgUrl: [
					{ url: 'other' },
					{ url: 'other' },
					{ url: 'other' },
					{ url: 'other' },
					{ url: 'other' },
					{ url: 'other' }
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

