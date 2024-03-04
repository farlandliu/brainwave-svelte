<script>
	import brainwave from '$lib/assets/brainwave.svg';
	import { navigation } from '$lib/constants';
	import Button from './Button.svelte';
</script>

<div
	class="fixed left-0 top-0 z-50 w-full border-b border-n-6 bg-n-8/90 backdrop-blur-sm lg:bg-n-8/90 lg:backdrop-blur-sm"
>
	<div class="flex items-center px-5 max-lg:py-4 lg:px-7.5 xl:px-10">
		<a class="block w-[12rem] xl:mr-8" href="#hero">
			<img src={brainwave} alt="Brainwave" />
		</a>
		<nav
			class="fixed bottom-0 left-0 right-0 top-[5rem] flex bg-n-8 lg:static lg:mx-auto lg:flex lg:bg-transparent"
		>
			<div class="relative z-2 m-auto flex flex-col items-center justify-center lg:flex-row">
				{#each navigation as item}
					{#if !item.onlyMobile}
						<a
							href={item.url}
							class="relative block px-6 py-6 font-code text-2xl uppercase text-n-1 transition-colors hover:text-color-1 md:py-8 lg:-mr-0.25 lg:text-xs lg:font-semibold lg:text-n-1/50 lg:hover:text-n-1"
							>{item.title}</a
						>
					{/if}
				{/each}
			</div>
		</nav>
		<a
			href="#signup"
			class="button mr-8 hidden text-n-1/50 transition-colors hover:text-n-1 lg:block"
		>
			New account
		</a>
		<Button className="hidden lg:flex" href="#login" >Sign in</Button>
	</div>
</div>
