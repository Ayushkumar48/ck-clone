<script>
	import { SearchOutline } from 'flowbite-svelte-icons';
	import NavLi from './NavLi.svelte';
	import NavIcon from './NavIcon.svelte';
	import HelloText from './HelloText.svelte';
	let navlis = ['About', 'Tools', 'Help'];
	let navIcons = ['fa-regular fa-message', 'fa-solid fa-gift', 'fa-solid fa-gear'];
</script>

<div
	class="flex h-[9%] w-full flex-row items-center justify-between border-b-4 border-black border-opacity-50 bg-white px-8 py-2 shadow-md"
>
	<div class="relative mr-4 flex h-10 w-full items-center justify-center">
		<div class="absolute left-0 flex h-full items-center justify-center pl-2">
			<SearchOutline />
		</div>
		<input type="text" placeholder="search..." class="h-full w-full rounded-xl px-9" />
	</div>
	<div class="flex flex-row gap-20">
		<div class="flex flex-row items-center justify-center gap-8">
			{#each navlis as navli}
				<NavLi>{navli}</NavLi>
			{/each}
		</div>
		<div class="flex flex-row items-center justify-center gap-8 rounded-sm px-2 py-1">
			{#each navIcons as navIcon}
				<NavIcon src={navIcon}></NavIcon>
			{/each}
		</div>
		<div class="flex items-center justify-center">
			<HelloText />
		</div>
	</div>
</div>
