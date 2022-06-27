<script>
	import { onMount } from 'svelte';

	let isShow = false;

	async function toggle() {
		isShow = !isShow;
	}
</script>

<nav class="top-0 sticky bg-white z-40">
	<div class="flex items-center justify-between md:py-6 lg:px-24 md:px-14 py-3 px-5 ">
		<a href="/" class="font-bold md:text-3xl text-xl underline"
			><span>HOTEL</span><span class="underline decoration-primary text-primary">MANIA</span></a
		>
		<div class="space-x-5 text- hidden md:block uppercase">
			<a class="nav-link" href="/">Home</a>
			<a class="nav-link" href="#services">Services</a>
			<a class="nav-link" href="#about">About Us</a>
			<a class="nav-link" href="#contact">Contact Us</a>
		</div>
		<div class="md:block hidden">
			<a
				href="/contact"
				class="uppercase bg-primary py-3 px-3 rounded-full text-white font-semibold border border-primary hover:bg-white hover:text-primary hover:transition-all"
				>Contact Us
			</a>
		</div>
		<div class="md:hidden visible">
			<button class="mobile-menu-button" on:click={toggle}>
				<svg
					class="w-7 h-7 ml-2 mt-1"
					xmlns="http://www.w3.org/2000/svg"
					fill="none"
					viewBox="0 0 24 24"
					stroke="currentColor"
				>
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="1.5"
						d="M4 6h16M4 12h16M4 18h16"
					/>
				</svg>
			</button>
		</div>
	</div>

	{#if isShow}
		<div class="space-y-2 text-sm px-4 py-4 mobile-menu md:hidden border-t border-t-primary -z-10">
			<a class="nav-menu" href="/about">About us</a>
			<a class="nav-menu" href="/businesses">Our Businesses</a>
			<!-- <a class="nav-menu" href="/message">MessageMe Service</a> -->
			<!-- <a class="nav-menu" href="/team">Our Team</a> -->
			<!-- <a class="nav-menu" href="/contact">Contact Us</a> -->
			<!-- <a class="nav-menu mb-2" href="faq">F.A.Qs</a> -->
			<a href="/contact" class="uppercase"
				><button class="bg-primary text-white py-1 text-left w-full border border-primary "
					>Contact Us Now</button
				></a
			>
		</div>
	{/if}
</nav>
