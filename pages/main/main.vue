<template>
	<view class="content">
		<!-- swiper -->
		<view class="uni-padding-wrap">
			<view class="page-section swiper">
				<view class="page-section-spacing">
					<swiper class="swiper" :indicator-dots="indicatorDots" :autoplay="autoplay" :interval="interval" :duration="duration">
						<swiper-item>
							<view class="swiper-item uni-bg-red">A</view>
						</swiper-item>
						<swiper-item>
							<view class="swiper-item uni-bg-green">B</view>
						</swiper-item>
						<swiper-item>
							<view class="swiper-item uni-bg-blue">C</view>
						</swiper-item>
					</swiper>
				</view>
			</view>
		</view>
		<!-- grid -->
		<uni-grid :options="[
			{image:'https://img-cdn-qiniu.dcloud.net.cn/img/shu.png',text:'院校库'},
			{image:'https://img-cdn-qiniu.dcloud.net.cn/img/lindang.png',text:'专业库'},
			{image:'https://img-cdn-qiniu.dcloud.net.cn/img/laoren.png',text:'排名库'},
			{image:'https://img-cdn-qiniu.dcloud.net.cn/img/laoren.png',text:'留学资讯'},
			{image:'https://img-cdn-qiniu.dcloud.net.cn/img/liwu.png',text:'问答'},]"
		 column-num="5">
		</uni-grid>
	</view>
</template>

<script>
	import {
		uniGrid
	} from '@dcloudio/uni-ui'

	export default {
		data() {
			return {
				background: ['color1', 'color2', 'color3'],
				indicatorDots: true,
				autoplay: true,
				interval: 2000,
				duration: 500
			}
		},
		components: {
			uniGrid
		},
		onLoad() {

		}
	}
</script>

<style>

</style>
