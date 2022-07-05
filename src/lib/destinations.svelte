<script>
	import { Swiper, SwiperSlide } from 'swiper/svelte';

	// Import Swiper styles
	import 'swiper/css';

	import '../style.css';

	import 'swiper/css/pagination';

	// import required modules
	import { Pagination } from 'swiper';
	import Destination from './destination.svelte';
</script>

<div class="mx-5 mt-20">
	<div class="space-y-3 text-center">
		<h3 class="h3">Our Popular <span class="text-primary">Destinations</span></h3>
		<p class="md:text-base text-sm">
			Our aim is to provide you with a top-quality tour experience.
		</p>
	</div>
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
			<SwiperSlide
				><Destination
					image="/beijing.png"
					title="Bangkok, Thailand."
					content="Bangkok is the capital and most populous city of Thailand. It is know in Thai as krung Thep Maha Nakhon or simply Krung Thep."
				/></SwiperSlide
			>
			<SwiperSlide
				><Destination
					image="/uk.png"
					title="Bangkok, Thailand."
					content="Bangkok is the capital and most populous city of Thailand. It is know in Thai as krung Thep Maha Nakhon or simply Krung Thep."
				/></SwiperSlide
			>
			<SwiperSlide
				><Destination
					image="/uss.png"
					title="Bangkok, Thailand."
					content="Bangkok is the capital and most populous city of Thailand. It is know in Thai as krung Thep Maha Nakhon or simply Krung Thep."
				/></SwiperSlide
			>
			<SwiperSlide
				><Destination
					image="/uss.png"
					title="Bangkok, Thailand."
					content="Bangkok is the capital and most populous city of Thailand. It is know in Thai as krung Thep Maha Nakhon or simply Krung Thep."
				/></SwiperSlide
			>
		</Swiper>
	</div>
</div>
