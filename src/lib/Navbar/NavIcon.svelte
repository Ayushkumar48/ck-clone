<script>
	import { onMount } from 'svelte';

	export let src = '';
	let svgContent = '';

	onMount(async () => {
		const response = await fetch(`${src}.svg`);
		svgContent = await response.text();
	});
	let fillColor = false;
</script>

<button
	class="flex items-center justify-center rounded-[0.2rem] bg-sky-300 p-2 shadow-md duration-150 ease-in-out hover:bg-[#e5871c4a]"
	on:mouseenter={() => (fillColor = true)}
	on:mouseleave={() => (fillColor = false)}
>
	<div class={`h-6 w-6 ${fillColor === true ? 'fill-[#E5871C]' : ''} duration-150 ease-in-out`}>
		<div
			class="svg-container h-full w-full opacity-70"
			contenteditable="false"
			bind:innerHTML={svgContent}
		></div>
	</div>
</button>
