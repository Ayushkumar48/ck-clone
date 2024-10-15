<script>
	import CustomerMap from './CustomerMap/CustomerMap.svelte';
	import QuickPersons from './QuickPersons/QuickPersons.svelte';
	import QuickStats from './QuickStats/QuickStats.svelte';
</script>

<div class="flex h-[91%] w-full flex-col gap-8 p-6">
	<div class="flex flex-col gap-1">
		<h1 class="text-3xl font-bold">Dashboard</h1>
		<p class="text-lg">Welcome to ChefKart Admin</p>
	</div>
	<div class="flex h-full w-full flex-col gap-4">
		<QuickStats />
		<QuickPersons />
		<CustomerMap />
	</div>
</div>
