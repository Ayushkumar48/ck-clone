<script>
	import '../app.css';
	import SideBar from '../lib/Sidebar/Sidebar.svelte';
	import Navbar from '../lib/Navbar/Navbar.svelte';
</script>

<div class="mb-72 flex h-screen w-full flex-row items-center justify-center bg-slate-200">
	<div class="flex h-full w-[18%] bg-slate-100">
		<SideBar />
	</div>
	<div class="flex h-full w-[82%] flex-col items-center justify-between">
		<Navbar />
		<slot></slot>
	</div>
</div>
