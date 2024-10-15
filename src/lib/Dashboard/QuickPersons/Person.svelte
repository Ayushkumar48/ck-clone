<script>
	export let person;
	import { goto } from '$app/navigation';
</script>

<tr
	class="bg-white shadow-sm duration-150 hover:cursor-pointer hover:bg-slate-100"
	on:click={() => goto(`/employees/${person.employeeId}`)}
>
	<td class="border px-4 py-2">{person.name}</td>
	<td class="border px-4 py-2">{person.employeeId}</td>
	<td class="border px-4 py-2">{person.position}</td>
	<td class="border px-4 py-2">{person.shiftTiming}</td>
	<td class="border px-4 py-2">{person.attendance}%</td>
	<td class="border px-4 py-2">{person.presentToday}</td>
	<td class="border px-4 py-2">{person.rating}/5.0</td>
</tr>
