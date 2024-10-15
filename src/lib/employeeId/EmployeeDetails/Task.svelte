<script>
	export let taskData;
</script>

<tr class="bg-white shadow-sm duration-150 hover:bg-slate-100">
	<td class="border px-4 py-2">{taskData.taskNo}</td>
	<td class="border px-4 py-2">{taskData.description}</td>
	<td class="border px-4 py-2">{taskData.givenAt}</td>
	<td class="border px-4 py-2">{taskData.dateGiven}</td>
	<td class="border px-4 py-2">{taskData.tableNo}</td>
	<td class="border px-4 py-2">{taskData.status}</td>
	<td class="border px-4 py-2">{taskData.remarks}</td>
</tr>
