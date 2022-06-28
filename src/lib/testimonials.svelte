<script>
	import Buttons from './buttons.svelte';
	import Testimonialcard from './testimonialcard.svelte';
</script>

<div class="mx-20">
	<div class="space-y-4 my-10 mb-16">
		<h3 class="h3">What our happy <span class="text-primary">Client</span> say</h3>
		<p class="text-center">Things that make it the best place to start trading</p>
	</div>
	<div class="grid grid-cols-3 my-10 gap-x-8">
		<Testimonialcard />
		<Testimonialcard />
		<Testimonialcard />
	</div>
	<Buttons />
</div>
