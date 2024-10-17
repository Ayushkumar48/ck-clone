<script>
	export let employeeId = 1;
</script>

<div class="flex h-full w-full flex-col justify-between gap-12 rounded-md bg-white p-4 shadow-lg">
	<div class="flex flex-row justify-between">
		<div class="text-2xl font-bold">
			Employee ID - {employeeId}
		</div>
		<div class="text-xl">Ratings - 4.2 / 5.0</div>
	</div>
	<div class="flex flex-row justify-between">
		<div class="flex flex-col gap-4">
			<div class="flex flex-row items-center gap-8">
				<div>
					<img
						src="/photo.jpg
					"
						alt="employee_photo"
						class="h-24 w-24"
					/>
				</div>
				<div class="flex flex-col gap-2">
					<div class="text-xl font-bold">Ayush Kumar</div>
					<div class="text-lg opacity-65">Chef</div>
				</div>
			</div>
			<div class="flex flex-col gap-4">
				<div class="flex flex-row items-center gap-2">
					<img src="/email.svg" alt="email" class="h-4 w-4" />
					<div>Email - ayush@gmail.com</div>
				</div>
				<div class="flex flex-row items-center gap-2">
					<img src="/phone.svg" alt="phone" class="h-4 w-4" />
					<div>Phone - 0123456789</div>
				</div>
			</div>
		</div>
		<table class="flex border-separate border-spacing-y-1 flex-col items-start justify-center">
			<tr>
				<th>Date of Joining -</th>
				<td>07/08/2022</td>
			</tr>
			<tr>
				<th>Shift Timings -</th>
				<td>9:00 to 18:00</td>
			</tr>
			<tr>
				<th>Attendance - </th>
				<td>92% / 100%</td>
			</tr>
			<tr>
				<th>Present Today? - </th>
				<td>Yes</td>
			</tr>
			<tr>
				<th>Total dishes served until now -</th>
				<td>40</td>
			</tr>
			<tr>
				<th>Speciality -</th>
				<td>Japanese Food</td>
			</tr>
		</table>
	</div>
</div>
