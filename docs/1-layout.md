# root div class

```html
## layout.svelte
<div class="overflow-hidden pt-[4.75rem] lg:pt-[5.25rem]"></div>
```

## components

### header

```html
<div
	class="fixed left-0 top-0 z-50 w-full  border-b border-n-6 bg-n-8/90 backdrop-blur-sm lg:bg-n-8/90 lg:backdrop-blur-sm"
>
	<div class="flex items-center px-5 max-lg:py-4 lg:px-7.5 xl:px-10">
		<h2>BrainWave</h2>
	</div>
</div>
```

### Hero

```html
<section class="-mt-[5.25rem] pt-[12rem]" id="hero">
	<div class="container relative">
		<div
			class="relative z-1 mx-auto mb-[3.875rem] max-w-[62rem] text-center md:mb-20 lg:mb-[6.25rem]"
		>
			<h1 class="h1 mb-6">Explore the Possibilities of&nbsp;AI&nbsp;Chatting</h1>
		</div>
	</div>
</section>
```

### Footer

```html
<section class="!px-0 !py-10">
	<div class="container flex items-center justify-center gap-10 max-sm:flex-col sm:justify-between">
		<p class="caption text-n-4 lg:block">© {new Date().getFullYear()}. All rights reserved.</p>
	</div>
</section>
```

## result

![layout](./img/1-layout.png)
