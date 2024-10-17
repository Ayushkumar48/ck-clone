<script>
	import { page } from '$app/stores';
	import EmployeeDetails from '../../../lib/employeeId/EmployeeDetails/EmployeeDetails.svelte';
	import Tasks from '../../../lib/employeeId/EmployeeDetails/Tasks.svelte';
	let employeeId = $page.params.id;
</script>

<article class="flex h-full w-full flex-col gap-6">
	<EmployeeDetails {employeeId} />
	<Tasks />
</article>
