<script>
	import { Swiper, SwiperSlide } from 'swiper/svelte';

	// Import Swiper styles
	import 'swiper/css';

	import 'swiper/css/pagination';
	import '../styless.css';

	// import required modules
	import { Pagination } from 'swiper';
	import Service from './service.svelte';
</script>

<div class="mt-20 mx-20">
	<div class="flex items-center space-x-5">
		<h3 class="h3-left w-[60%]">Choose your <span class="text-primary">luxurious</span> room</h3>
		<p class="pr-80 text-sm">
			At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiss praesentium
			voluptatum deleniti atque corrupti quos dolores
		</p>
	</div>

	<div class="">
		<div>
			<Swiper
				slidesPerView={1}
				spaceBetween={10}
				pagination={{
					clickable: true
				}}
				breakpoints={{
					'640': {
						slidesPerView: 1,
						spaceBetween: 20
					},
					'768': {
						slidesPerView: 2,
						spaceBetween: 40
					},
					'1024': {
						slidesPerView: 3,
						spaceBetween: 50
					}
				}}
				modules={[Pagination]}
				class="mySwiper"
			>
				<SwiperSlide><Service image="/service1.jpg" title="" content="" /></SwiperSlide>
				<SwiperSlide><Service image="/service2.jpg" title="" content="" /></SwiperSlide>
				<SwiperSlide><Service image="/service3.jpg" title="" content="" /></SwiperSlide>
				<SwiperSlide><Service image="/service1.jpg" title="" content="" /></SwiperSlide>
				<SwiperSlide><Service image="/service2.jpg" title="" content="" /></SwiperSlide>
				<SwiperSlide><Service image="/service3.jpg" title="" content="" /></SwiperSlide>
				<SwiperSlide><Service image="/service1.jpg" title="" content="" /></SwiperSlide>
			</Swiper>
		</div>
	</div>
</div>
