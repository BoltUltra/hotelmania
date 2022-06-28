<script>
	import Testimonialcard from './testimonialcard.svelte';
	import { Swiper, SwiperSlide } from 'swiper/svelte';

	// Import Swiper styles
	import 'swiper/css';

	import 'swiper/css/pagination';
	import '../stylessc.css';

	// import required modules
	import { Pagination } from 'swiper';
</script>

<div class="mt-20 mx-20">
	<div class="space-y-4 my-10">
		<h3 class="h3">What our happy <span class="text-primary">Client</span> say</h3>
		<p class="text-center">Things that make it the best place to start trading</p>
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
				<SwiperSlide
					><div class="shadow-lg rounded-lg relative text-center py-6 px-4 bg-[#F9FAFB]">
						<div class="-top-14 relative">
							<img src="/testimonial.jpg" alt="" class="rounded-full w-20 mx-auto" />
							<p class="text-[#FDCC0D]">
								<i class="fa-solid fa-star" />
								<i class="fa-solid fa-star" />
								<i class="fa-solid fa-star" />
								<i class="fa-solid fa-star" />
								<i class="fa-solid fa-star" />
							</p>
							<h4 class="font-bold">Jane Doe</h4>
						</div>
						<p class="text-sm">
							Okay, I’ve found the joy of cooking. It’s the process which my better half does it.
							There is ncere love than the adoration for sustenance.
						</p>
					</div></SwiperSlide
				>
			</Swiper>
		</div>
	</div>
</div>
