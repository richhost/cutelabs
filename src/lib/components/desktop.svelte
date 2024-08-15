<script lang="ts">
	const list = [
		{
			name: 'PixZip',
			description: 'Easy-to-use image compression software.',
			icon: 'https://pixzip.cutelabs.in/_next/image?url=%2Ficon.webp&w=256&q=100',
			link: 'https://pixzip.cutelabs.in',
			price: '$9.9'
		},
		{
			name: 'Happy Times',
			description: '给摸鱼做个统计',
			icon: 'https://is1-ssl.mzstatic.com/image/thumb/Purple211/v4/17/c1/76/17c17667-1925-d9c8-3b3a-595146591452/AppIcon-0-0-85-220-0-4-0-2x.png/460x0w.webp',
			link: 'https://apps.apple.com/us/app/happy-times/id6497649329',
			iconClass: 'w-16',
			price: '$0.99'
		}
	];
</script>

<section class="mt-10">
	<h3 class="text-xl font-bold mb-2">Desktop</h3>

	<div class="grid gird-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-5">
		{#each list as item}
			<div class="flex items-center gap-2">
				<img class="w-14 aspect-square {item.iconClass}" src={item.icon} alt="icon" />
				<div class="grow">
					<div class="font-medium">{item.name}</div>
					<div class="text-secondary text-sm leading-tight">{item.description}</div>
					<div class="divider my-0"></div>
				</div>
				<a class="btn btn-sm w-14 btn-info" target="_blank" rel="noreferrer" href={item.link}
					>{item.price}</a
				>
			</div>
		{/each}
	</div>
</section>
