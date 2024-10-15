<script>
	export let info;
</script>

<div class="inline-block h-full w-[50%] animate-bounce space-y-1">
	<div class="flex h-full w-full flex-row items-center gap-8 rounded-2xl bg-white p-6 shadow-md">
		<div class="flex items-center justify-center rounded-full bg-slate-200 p-4">
			<img src="dollar.svg" alt="" class="h-8 w-8" />
		</div>
		<div>
			<div class="text-md">
				{info.title}
			</div>
			<div class="text-2xl font-bold">{info.num}</div>
			<div class="text-sm opacity-50">( past 30 days )</div>
		</div>
	</div>
</div>
