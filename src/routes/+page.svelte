<script>
	import { MetaTags } from 'svelte-meta-tags';
	import Browser from '$lib/components/browser.svelte';
	import Desktop from '$lib/components/desktop.svelte';
</script>

<MetaTags title="Cute Lab - Make your online life better." />

<hgroup>
	<h1 class="text-xl font-bold">Welcome to Cute Labs</h1>
	<p class="text-secondary">Make your online life better.</p>
</hgroup>

<Desktop />
<Browser />
