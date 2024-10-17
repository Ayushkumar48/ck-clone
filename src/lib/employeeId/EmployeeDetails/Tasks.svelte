<script>
	import Task from './Task.svelte';

	let tasksData = [
		{
			taskNo: 1,
			description: 'Make a good Sushi with different Sauces.',
			givenAt: '14:25',
			dateGiven: '14/08/2024',
			tableNo: 12,
			status: 'Completed',
			remarks: 'Good Food'
		},
		{
			taskNo: 2,
			description: 'Make a good Sushi with different Sauces.',
			givenAt: '14:25',
			dateGiven: '14/08/2024',
			tableNo: 12,
			status: 'Completed',
			remarks: 'Good Food'
		},
		{
			taskNo: 3,
			description: 'Make a good Sushi with different Sauces.',
			givenAt: '14:25',
			dateGiven: '14/08/2024',
			tableNo: 12,
			status: 'Completed',
			remarks: 'Good Food'
		},
		{
			taskNo: 4,
			description: 'Make a good Sushi with different Sauces.',
			givenAt: '14:25',
			dateGiven: '14/08/2024',
			tableNo: 12,
			status: 'Completed',
			remarks: 'Good Food'
		}
	];
</script>

<div class="rounded-lg bg-white p-4 shadow-lg">
	<table class="w-full border-separate border-spacing-y-4">
		<thead>
			<tr>
				<th class="text-left">Task No.</th>
				<th class="text-left">Description</th>
				<th class="text-left">Given at</th>
				<th class="text-left">Date given</th>
				<th class="text-left">Table No.</th>
				<th class="text-left">Status</th>
				<th class="text-left">Remarks from customer</th>
			</tr>
		</thead>
		<tbody>
			{#each tasksData as taskData}
				<Task {taskData} />
			{/each}
		</tbody>
	</table>
</div>
