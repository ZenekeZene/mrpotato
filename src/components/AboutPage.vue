<template>
	<article class="face-wrapper">
		<section class="block"></section>
		<ul>
			<li class="item front">Front</li>
			<li class="item eye --left">Ojo</li>
			<li class="item eye --right">Ojo</li>
			<li class="item nose">Nariz</li>
			<li class="item mouth">Boca</li>
		</ul>
		<swiper :options="swiperOptionPieces" class="pieces-swiper">
			<swiper-slide>1</swiper-slide>
			<swiper-slide>2</swiper-slide>
			<swiper-slide>3</swiper-slide>
			<swiper-slide>4</swiper-slide>
			<swiper-slide>5</swiper-slide>
			<swiper-slide>6</swiper-slide>
			<swiper-slide>7</swiper-slide>
			<swiper-slide>8</swiper-slide>
			<swiper-slide>9</swiper-slide>
			<swiper-slide>10</swiper-slide>
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
				swiperOptionPieces: {
					centeredSlides: false,
					slidesPerView: 5,
				},
			};
		},
	};
</script>
