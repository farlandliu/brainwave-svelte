<script>
	import '../app.pcss';
	import Header from '$lib/components/Header.svelte';
	import Hero from '$lib/components/Hero.svelte';
	import Footer from '$lib/components/Footer.svelte';
</script>
<div class="pt-[4.75rem] lg:pt-[5.25rem] overflow-hidden">
	<Header />
	<Hero />
	<slot />
	<Footer />
</div>

