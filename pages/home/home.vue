<template name="homeSwapper">
	<view class="page-section-spacing">熱污染群二無群二無群二
		<!-- <swiper class="swiper" :indicator-dots="indicatorDots" :autoplay="autoplay" :interval="interval" :duration="duration">
			<swiper-item><view class="swiper-item uni-bg-red">A</view></swiper-item>
			<swiper-item><view class="swiper-item uni-bg-green">B</view></swiper-item>
			<swiper-item><view class="swiper-item uni-bg-blue">C</view></swiper-item>
		</swiper> -->
	</view>
</template>
 
<script>
export default {
	name: 'homeSwapper',
	data() {
		return {
			autoplay: true,
			interval: 3000,
			duration: 500,
			title: '轮播图'
		};
	}
};
</script>
 
<style>
.swiper {
	width: 100%;
	height: 300px;
}
.swiper-item {
	width: 100%;
	height: 100%;
}
.uni-bg-red {
	background: red;
}
.uni-bg-green {
	background: #4cd964;
}
.uni-bg-blue {
	background: #007aff;
}
</style>