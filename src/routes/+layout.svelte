<script>
	import '../app.pcss';
	import Header from '$lib/components/Header.svelte';
	import Hero from '$lib/components/Hero.svelte';
	import Footer from '$lib/components/Footer.svelte';
	import ButtonGradient from '$lib/components/ButtonGradient.svelte';
</script>

<div class="overflow-hidden pt-[4.75rem] lg:pt-[5.25rem]">
	<Header />
	<slot />
	<Footer />
</div>
<ButtonGradient />
