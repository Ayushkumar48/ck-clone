<script>
	import Employees from '../../lib/employees/Employees.svelte';
	import { Button } from 'flowbite-svelte';
</script>

<div class="flex flex-col gap-4">
	<Employees />
	<div class="flex justify-between px-40 pb-8">
		<Button color="light">Previous</Button>
		<Button color="light">Next</Button>
	</div>
</div>
