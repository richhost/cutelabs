<script lang="ts">
	const list = [
		{
			name: 'One Tab Flow',
			description: "Quickly switch your browser's new tab.",
			link: 'https://chromewebstore.google.com/detail/one-tab-flow/hgaihhepaknebghekjfbjhpbpjlfheok',
			icon: 'https://lh3.googleusercontent.com/iHSadh7VyVYw-fIYBfoqhXjoGDVkluudrM4-Sh5xEv4_Z_FFxFzr6JK8sotoRrknsLeatyT4C5K8tD1QEQSf7Wnm5Xg=s120',
			price: 'Free'
		}
	];
</script>

<section class="mt-10">
	<h3 class="text-xl font-bold mb-2">Chrome Extension</h3>

	<div class="grid gird-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-5">
		{#each list as item}
			<div class="flex items-center gap-2">
				<img class="w-14 aspect-square" src={item.icon} alt="icon" />
				<div class="grow">
					<div class="font-medium">{item.name}</div>
					<div class="text-secondary text-sm leading-tight">{item.description}</div>
					<div class="divider my-0"></div>
				</div>
				<a class="btn btn-sm btn-info w-14" target="_blank" rel="noreferrer" href={item.link}
					>{item.price}</a
				>
			</div>
		{/each}
	</div>
</section>
