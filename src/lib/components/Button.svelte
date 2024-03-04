<script lang="ts">
  import ButtonSvg from "./ButtonSvg.svelte";
  export let white:boolean = false;
  export let px:string = "px-7";
  export let href:string = "";
  export let className:string = "";

</script>

{#if href}
<a
href="{href}"
class="button relative inline-flex items-center justify-center h-11 transition-colors hover:text-color-1  { px }
 {white ? "text-n-8" : "text-n-1"}
  {className}">
 <span class="relative z-10"><slot /></span>
 <ButtonSvg {white} />
 </a>
{:else}
	button
{/if}

