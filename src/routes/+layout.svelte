<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';

	import { resolveRoute } from '$app/paths';
	let { children } = $props();
</script>

<nav>
    <a href={resolveRoute('/')}>home</a>
	<a href={resolveRoute('/blog')}>blog</a>
	<a href={resolveRoute('/about')}>about</a>
</nav>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>
{@render children()}
