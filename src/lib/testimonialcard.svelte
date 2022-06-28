<script>
	export let image = '/testimonial.jpg';
	export let user = 'Jane Doe';
	export let content =
		'Okay, I’ve found the joy of cooking. It’s the process which my better half does it. There is sincere love than the adoration for sustenance.';
</script>

<div>
	<div class="shadow-lg hover:shadow-xl rounded-lg relative text-center py-6 px-4 bg-[#F9FAFB]">
		<div class="-top-14 -mb-10 relative">
			<img src={image} alt="" class="rounded-full w-20 mx-auto" />
			<p class="text-[#FDCC0D]">
				<i class="fa-solid fa-star" />
				<i class="fa-solid fa-star" />
				<i class="fa-solid fa-star" />
				<i class="fa-solid fa-star" />
				<i class="fa-solid fa-star" />
			</p>
			<h4 class="font-bold">{user}</h4>
		</div>
		<p class="text-sm">
			{content}
		</p>
	</div>
</div>
