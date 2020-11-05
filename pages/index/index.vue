<template>
	<view class="container">
		<view class="container-content">
			I AM DESIGNER! GHENYUE.
		</view>
		<navigator url="../content/content" class="container-btn">
			<button>开始</button>
		</navigator>
		<!-- <contentPage></contentPage> -->
	</view>
</template>

<script>
	import contentPage from '../content/content.vue';
	export default {
		data() {
			return {}
		},
		components: {
			contentPage
		},
		methods: {

		}
	}
</script>

<style>
	.container {
		font-size: 14px;
		line-height: 24px;
		width: 100%;
		min-height: 500px;
		display: flex;
		flex-flow: column;
		justify-content: space-between;
		align-items: center;
	}

	.container-content {
		padding-top: 80px;
		font-size: 22px;
		color: #D3D3D3;
		font-weight: 700;
	}

	.container-btn {
		max-width: 380px;
		width: 100%;
		font-size: 22px;
		font-weight: 700;
	}
</style>
