<script>
	export let image = '';
	export let content = '';
	export let title = '';
</script>

<div
	class="shadow-xl rounded md:my-9 mb-9 md:mx-0 mx-3 px-3 py-10 md:py-22 md:w-full md:overflow-hidden"
>
	<div class="rounded">
		<img src={image} alt="" class="rounded" />
	</div>
	<div class="mt-5">
		<h4 class="text-lg font-bold text-primary mb-3">{title}</h4>
		<p class="text-sm">{content}</p>
	</div>
</div>
