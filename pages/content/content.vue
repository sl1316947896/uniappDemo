<template name="content">
	<view class="content-cont">
		<view class="cont-title">
			<h2>POINT VISION</h2>
		</view>
		<view class="cont-about-me">
			<view class="about-me-left">
				<view class="about-me-title">About me</view>
				<view class="about-me-center">个人简历</view>
				<view class="about-me-cont">
					<text>{{personalInformation.school}}</text>
					<text>{{personalInformation.schoolHours}}</text>
					<text>{{personalInformation.college}}</text>
				</view>
			</view>
			<view class="about-me-right">
				<image class="about-me-right-img" src="../../static/images/chenyue.jpg"></image>
			</view>
		</view>
		<view v-for="(i,key) in data" :key="key" class="cont-items" @click="onClick($event, key)">
			<view class="items-title">
				{{i.itemName}}
			</view>
			<view class="items-cont">
				{{i.itemContent}}
			</view>
		</view>
	</view>
</template>

<script>
	import data from '../../static/data.js';

	export default {
		name: 'contentPage',
		data() {
			return {
				data: data.data,
				personalInformation: data.personalInformation
			};
		},
		methods: {
			onClick: (e, key) => {
				console.log(e, key, 90)
			},
		}
	}
</script>

<style>
	.content-cont {
		padding: 0 12px;
	}

	.cont-title {
		margin-bottom: 12px;
		color: #ead8ff;
		font-size: 18px;
	}

	.cont-about-me {
		background-image: linear-gradient(#ba45ff, #6a38cb);
		color: #f2eaff;
		border-radius: 5px;
		margin-bottom: 10px;
		height: 107px;
		display: flex;
		justify-content: space-between;
	}

	.about-me-left {
		display: flex;
		flex-flow: column;
		justify-content: center;
		font-size: 12px;
		padding: 15px;
	}

	.about-me-right {
		height: 100%;
		width: 80px;
	}
	.about-me-right-img{
		width: 100%;
		height: 100%;
		border-radius: 0 0 0 100px;
	}
	.about-me-center {
		margin-top: 28px;
	}

	.about-me-title {}

	.about-me-cont {
		margin-top: 6px;
		font-size: 8px;
	}

	.cont-items {
		margin-bottom: 10px;
		background-color: #fff;
		color: #333333;
		border-radius: 5px;
		padding: 10px 20px;
		height: 107px;
		background-image: linear-gradient(#f21c79, #5a1f5c);
		display: flex;
		flex-flow: column;
		justify-content: center;
	}

	.items-title {
		color: #e9d7fe;
		font-size: 14px;
	}

	.items-cont {
		color: #d4a5d5;
		font-size: 8px;
		margin-top: 11px;
	}
</style>
