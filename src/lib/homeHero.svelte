<script>
	import Searchmenu from './searchmenu.svelte';
</script>

<div>
	<div
		class="md:grid md:grid-cols-5 md:place-items-center relative md:mx-20 mx-5 md:mt-0 mt-10 space-y-3 text-center md:text-left"
	>
		<div class="col-span-2 md:space-y-0 space-y-3">
			<p class="text-[#DEBF8D] md:text-sm text-xs">FIND YOUR DREAM HOTEL</p>
			<h2 class="md:text-[58px] text-4xl font-semibold leading-tight">
				Your <span class="text-primary">Dream</span> Hotel is Waiting for You!
			</h2>
			<p class="text-sm md:mr-[170px] font-semibold">
				Find Hotels, rooms and Houses for your stay all around the globe and make your trips more
				exciting....
			</p>
			<Searchmenu />
			<p class="md:text-sm font-semibold">Top Locations: Manchester, London, Greenwich</p>
		</div>
		<div class="col-span-3">
			<img src="/heroimg.png" alt="" />
		</div>
	</div>
</div>
