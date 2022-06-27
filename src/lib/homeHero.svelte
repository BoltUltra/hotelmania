<script>
	import Searchmenu from './searchmenu.svelte';
</script>

<div>
	<div class="grid grid-cols-5 md:place-items-center relative mx-20 space-y-3">
		<div class="col-span-2">
			<p class="text-[#DEBF8D] text-sm">FIND YOUR DREAM HOTEL</p>
			<h2 class="text-[58px] font-semibold leading-tight">
				Your <span class="text-primary">Dream</span> Hotel is Waiting for You!
			</h2>
			<p class="text-sm mr-[170px] font-semibold">
				Find Hotels, rooms and Houses for your stay all around the globe and make your trips more
				exciting....
			</p>
			<Searchmenu />
			<p class="text-sm font-semibold">Top Locations: Manchester, London, Greenwich</p>
		</div>
		<div class="col-span-3">
			<img src="/heroimg.png" alt="" />
		</div>
	</div>
</div>
