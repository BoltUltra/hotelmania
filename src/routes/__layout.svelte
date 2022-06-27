<script>
	import Footer from './../lib/footer.svelte';
	import Navbar from './../lib/navbar.svelte';
	import '../app.css';
	import '../style.css';
</script>

<Navbar />
<main>
	<slot />
</main>
<Footer />
