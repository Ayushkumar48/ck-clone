<script>
	import '../app.css';
	import SideBar from '$lib/Sidebar/Sidebar.svelte';
	import Navbar from '$lib/Navbar/Navbar.svelte';
</script>

<div class="mb-72 flex h-screen w-full flex-row items-center justify-center">
	<div class="flex h-full w-[18%] rounded-lg bg-slate-100 shadow-lg">
		<SideBar />
	</div>
	<div class="flex h-full w-[82%] flex-col items-center justify-between">
		<Navbar />
		<div class="h-full w-full p-4">
			<slot></slot>
		</div>
	</div>
</div>
