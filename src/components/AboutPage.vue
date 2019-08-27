<template>
	<article class="face-wrapper">
		<section class="block"></section>
		<swiper :options="swiperOption">
			<swiper-slide>I'm Slide 1</swiper-slide>
			<swiper-slide>I'm Slide 2</swiper-slide>
		</swiper>
		<swiper :options="swiperOption">
			<swiper-slide>I'm Slide 1</swiper-slide>
			<swiper-slide>I'm Slide 2</swiper-slide>
		</swiper>
		<swiper :options="swiperOption">
			<swiper-slide>I'm Slide 1</swiper-slide>
			<swiper-slide>I'm Slide 2</swiper-slide>
		</swiper>
		<swiper :options="swiperOption">
			<swiper-slide>I'm Slide 1</swiper-slide>
			<swiper-slide>I'm Slide 2</swiper-slide>
		</swiper>

		<swiper :options="swiperOptionVertical" class="swiper-vertical">
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
