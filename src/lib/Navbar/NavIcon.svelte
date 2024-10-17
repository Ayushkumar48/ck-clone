<script>
	export let src;
	let fillColor = false;
</script>

<button
	class="flex items-center justify-center rounded-[0.2rem] bg-sky-300 p-2 shadow-md duration-150 ease-in-out hover:bg-[#e5871c4a]"
	on:mouseenter={() => (fillColor = true)}
	on:mouseleave={() => (fillColor = false)}
>
	<i class={src + ' ' + 'flex h-6 w-6 items-center justify-center duration-150 ease-in-out'}></i>
</button>
