<script>
	import ListItems from './ListItems.svelte';
	import Title from './Title.svelte';
	let arr = ['Dashboard', 'Orders', 'Menus', 'Customers'];
</script>

<div class="flex h-full w-full flex-col gap-8 bg-white px-4 py-4">
	<div>
		<div class="bg-black">
			<Title />
		</div>
		<h2 class="text-center text-3xl font-bold">Admin Panel</h2>
	</div>
	<ul class="flex w-full flex-col">
		{#each arr as a}
			<ListItems>{a}</ListItems>
		{/each}
	</ul>
</div>
