<script>
	import Stat from './Stat.svelte';

	let ordersData = [
		{
			title: 'Total Orders',
			num: '200K'
		},
		{
			title: 'Total Revenue',
			num: '150K'
		}
	];
</script>

<div class="flex flex-row justify-around gap-4">
	{#each ordersData as order}
		<Stat info={order} />
	{/each}
</div>
