<template>
	<article class="face-wrapper">
		<ul class="face">
			<li class="item front --back"></li>
			<li class="atrezzo middle"></li>
			<li class="item back --back"></li>
			<li class="item hair bg-template"></li>
			<li class="item hat bg-template"></li>
			<li class="item eyebrown --left bg-template"></li>
			<li class="item eyebrown --right bg-template"></li>
			<li class="item eye --left"></li>
			<li class="item eye --right"></li>
			<li class="item ear --left"></li>
			<li class="item ear --right"></li>
			<li class="item nose bg-template"></li>
			<li class="item mouth bg-template"></li>
			<li class="atrezzo body bg-template"></li>
			<li class="atrezzo neck"></li>
		</ul>
		<swiper :options="swiperOptionPieces" class="pieces-swiper">
			<swiper-slide>
				<div class="box">1</div>
			</swiper-slide>
			<swiper-slide>
				<div class="box">2</div>
			</swiper-slide>
			<swiper-slide>
				<div class="box">3</div>
			</swiper-slide>
			<swiper-slide>
				<div class="box">4</div>
			</swiper-slide>
			<swiper-slide>
				<div class="box">5</div>
			</swiper-slide>
			<swiper-slide>
				<div class="box">6</div>
			</swiper-slide>
			<swiper-slide>
				<div class="box">7</div>
			</swiper-slide>
			<swiper-slide>
				<div class="box">8</div>
			</swiper-slide>
			<swiper-slide>
				<div class="box">9</div>
			</swiper-slide>
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
