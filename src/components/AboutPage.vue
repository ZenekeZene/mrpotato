<template>
	<article style="width: 100%; height: 100%; border: 2px solid red;">
		<swiper ref="mySwiper" :options="swiperOption">
			<swiper-slide>I'm Slide 1</swiper-slide>
			<swiper-slide>I'm Slide 2</swiper-slide>
		</swiper>
		<swiper ref="mySwiper" :options="swiperOption">
			<swiper-slide>I'm Slide 1</swiper-slide>
			<swiper-slide>I'm Slide 2</swiper-slide>
		</swiper>
		<swiper ref="mySwiper" :options="swiperOption">
			<swiper-slide>I'm Slide 1</swiper-slide>
			<swiper-slide>I'm Slide 2</swiper-slide>
		</swiper>
		<swiper ref="mySwiper" :options="swiperOption">
			<swiper-slide>I'm Slide 1</swiper-slide>
			<swiper-slide>I'm Slide 2</swiper-slide>
		</swiper>
		<swiper ref="mySwiper" :options="swiperOption">
			<swiper-slide>I'm Slide 1</swiper-slide>
			<swiper-slide>I'm Slide 2</swiper-slide>
		</swiper>

		<swiper ref="mySwiper" :options="swiperOptionVertical" class="swiper-vertical">
			<swiper-slide>I'm Slide 1</swiper-slide>
			<swiper-slide>I'm Slide 2</swiper-slide>
		</swiper>
	</article>
</template>

<script>

	export default {
		name: 'AboutPage',
		data() {
			return {
				swiperOption: {
					centeredSlides: true,
					slidesPerView: 1,
				},
				swiperOptionVertical: {
					direction: 'vertical',
					centeredSlides: true,
					slidesPerView: 1,
				},
			};
		},
	};
</script>
<style lang="scss">
	.swiper-slide {
		height: calc(100vh / 6);
		border: 2px solid green;
	}

	.swiper-vertical {
		position: absolute;
		top: 20vh;
		left: 50%;
		z-index: 1;
		width: 28vw;
		height: 23vh;
		transform: translate3D(-50%, 50%, 0);

		.swiper-slide {
			height: 100vh;
			border: 2px solid black;
		}
	}

</style>