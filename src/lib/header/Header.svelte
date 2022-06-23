<script>
	import { page } from '$app/stores';
	import logo from './svelte-logo.svg';
</script>

<header>


	<nav class="grid grid-cols-2 items-center w-[100vw] px-[10%] py-3">
	<div class="flex items-center">
		<a href="https://kit.svelte.dev">
			<img class="w-[2rem]" src={logo} alt="SvelteKit" />

		</a>
		 	<h1 class="text-xl font-black">Svelte
	</div>
		<ul class="flex justify-end">
			<li class:active={$page.url.pathname === '/'}><a sveltekit:prefetch href="/" class="ml-8 uppercase font-bold">Home</a></li>
			<li class:active={$page.url.pathname === '/about'}>
				<a sveltekit:prefetch href="/about" class="ml-8 uppercase font-bold">About</a>
			</li>
			<li class:active={$page.url.pathname === '/contact'}>
				<a sveltekit:prefetch href="/contact" class="ml-8 uppercase font-bold">Contact</a>
			</li>
		</ul>
	
</header>

<style>



	






</style>
