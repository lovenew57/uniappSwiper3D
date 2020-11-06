# uniappSwiper3D
一个开源的Uniapp的3d轮播组件


重要参数说明：

	imgList : 一个数组，存放轮播图片的src地址 和准备跳转的url地址 如果不填url 就是不跳转  也可以缺省url参数表示不跳转
	 例子：
	imgList: [
	{url: 'other?id=1' , src: '../../static/winbox.png' },
	{url: '' , src: '../../static/winbox.png' },
	{url: '' , src: '../../static/winbox.png' },
	{url: '' , src: '../../static/winbox.png' },
	{url: 'other?id=2' , src: '../../static/winbox.png' },
	],	
    
    haveUrl : { type : Boolean, default : true },//是否进行页面的跳转
    特别说明：默认是true 如果不进行跳转 不传imgUrl或者直接设置fales也可以
    
    
    
		currentIndexParameter  : {type : Number, default : 1},//默认放在中间的图片
		movewidthParameter  : {type : Number, default : 0.4},//图片位移
		openTypeParameter  :{type : String, default : "navigate"},//switchTab 也是是去tabbar页面 普通页面为navigate 


使用例子详见 index.vue


