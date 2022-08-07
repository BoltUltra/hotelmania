<script>
	import Buttons from './buttons.svelte';
	import Testimonialcard from './testimonialcard.svelte';
</script>

<div class="md:mx-20 mx-10">
	<div class="space-y-4 my-10 mb-16">
		<h3 class="h3">What our happy <span class="text-primary">Client</span> say</h3>
		<p class="text-center">Things that make it the best place to start trading</p>
	</div>
	<div class="md:grid md:grid-cols-3 my-10 md:gap-x-8 md:space-y-0 space-y-14" data-aos="fade-up">
		<Testimonialcard />
		<Testimonialcard />
		<Testimonialcard />
	</div>
	<div class="md:visible invisible">
		<Buttons />
	</div>
</div>
