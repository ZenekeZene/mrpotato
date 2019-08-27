<template>
	<article class="face-wrapper">
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
					effect: 'cube',
					grabCursor: true,
					cubeEffect: {
						shadow: false,
						slideShadows: true,
						shadowOffset: 0,
						shadowScale: 1
					},
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
	.swiper-slide,
	.swiper-container-cube .swiper-slide {
		display: flex;
		justify-content: center;
		align-items: center;
		height: calc(100vh / 6);
		border: 1px dashed green;
	}

	.swiper-container-cube {
		perspective: none;
	}

	.swiper-vertical {
		position: absolute;
		top: 20vh;
		left: 50%;
		z-index: 1;
		width: 28vw;
		height: 23vh;
		transform: translate3D(-50%, 50%, 0);
	}

</style>