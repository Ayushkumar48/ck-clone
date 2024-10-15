<!-- src/routes/employees/[id]/+page.svelte -->
<script>
	import { page } from '$app/stores';
	let employeeId = $page.params.id;

	// Fetch or display employee-specific data using employeeId
</script>

<article>
	<h1>Employee Details for {employeeId}</h1>
	<!-- Your content here -->
</article>
