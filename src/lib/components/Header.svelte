<script>
	import Nav from './Nav.svelte';
	import Hero from './Hero.svelte';
	import { page } from '$app/stores';
</script>

<header>
	<Nav />
	{#if $page.url.pathname === '/' || $page.url.pathname === ''}
		<Hero></Hero>
	{/if}
</header>

