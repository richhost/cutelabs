<script lang="ts">
	import type { Snippet } from 'svelte';
	import '../app.css';
	import Header from '$lib/components/header.svelte';

	const { children }: { children: Snippet } = $props();
</script>

<div class="max-w-7xl px-5 mx-auto">
	<Header />
	{@render children()}
</div>
