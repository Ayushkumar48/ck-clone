<script>
	import BarChart from '../../Charts/BarChart.svelte';
	import Line from '../../Charts/Line.svelte';
	import PieChart from '../../Charts/PieChart.svelte';
</script>

<div class="flex h-full w-full flex-row justify-between gap-8 rounded-xl bg-white p-4 shadow-lg">
	<div class="w-full">
		<BarChart />
	</div>
	<div class="w-full">
		<!-- <PieChart /> -->
		<Line />
	</div>
</div>
