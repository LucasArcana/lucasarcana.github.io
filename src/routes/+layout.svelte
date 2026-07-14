<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';

	import { resolve } from '$app/paths';
	let { children } = $props();
</script>

<nav class="topnav">
    <a href={resolve('/')}>home</a>
	<a href={resolve('/blog')}>blog</a>
	<a href={resolve('/about')}>about</a>
</nav>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>
{@render children()}
