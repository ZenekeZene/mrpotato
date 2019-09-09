<template>
	<article class="face-wrapper">
		<ul class="face">
			<li class="item front"></li>
			<li class="item middle"></li>
			<li class="item back"></li>
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
			<li class="atrezzo neck bg-template"></li>
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
