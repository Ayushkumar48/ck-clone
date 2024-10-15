<script>
	import Person from './Person.svelte';

	let personData = [
		{
			name: 'Ayush Kumar',
			employeeId: 12345,
			position: 'Chef',
			shiftTiming: '9:00-18:00',
			attendance: 92,
			presentToday: 'Yes',
			rating: 4.2
		},
		{
			name: 'Ayush Kumar',
			employeeId: 12345,
			position: 'Chef',
			shiftTiming: '9:00-18:00',
			attendance: 92,
			presentToday: 'Yes',
			rating: 4.2
		},
		{
			name: 'Ayush Kumar',
			employeeId: 12345,
			position: 'Janitor',
			shiftTiming: '9:00-18:00',
			attendance: 92,
			presentToday: 'Yes',
			rating: 4.2
		},
		{
			name: 'Ayush Kumar',
			employeeId: 12345,
			position: 'Maid',
			shiftTiming: '9:00-18:00',
			attendance: 100,
			presentToday: 'Yes',
			rating: 4.2
		},
		{
			name: 'Ayush Kumar',
			employeeId: 12345,
			position: 'Maid',
			shiftTiming: '9:00-18:00',
			attendance: 100,
			presentToday: 'Yes',
			rating: 4.2
		}
	];
</script>

<div class="w-full rounded-xl bg-white p-4 shadow-lg">
	<table class="w-full border-separate border-spacing-y-4">
		<thead>
			<tr>
				<th class="text-left">Name</th>
				<th class="text-left">Employee ID</th>
				<th class="text-left">Position</th>
				<th class="text-left">Shift Timing</th>
				<th class="text-left">Attendance</th>
				<th class="text-left">Present Today?</th>
				<th class="text-left">Rating</th>
			</tr>
		</thead>
		<tbody>
			{#each personData as person}
				<Person {person} />
			{/each}
		</tbody>
	</table>
</div>
