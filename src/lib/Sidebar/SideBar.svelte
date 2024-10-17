<script>
	import ListItems from './ListItems.svelte';
	let arr = [
		{
			name: 'Dashboard',
			src: '/'
		},
		{
			name: 'Orders',
			src: '/'
		},
		{
			name: 'Menus',
			src: '/'
		},
		{
			name: 'Customers',
			src: '/'
		},
		{
			name: 'Employees',
			src: '/employees'
		}
	];
</script>

<div class="flex w-full flex-col gap-8 rounded-br-lg bg-white px-4 py-4">
	<a href="/">
		<h2 class="text-center text-3xl font-bold">Admin Panel</h2>
	</a>
	<ul class="flex w-full flex-col">
		{#each arr as content}
			<ListItems {content}></ListItems>
		{/each}
	</ul>
</div>
