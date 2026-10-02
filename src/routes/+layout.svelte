<script>
	import './layout.css';
	let { children } = $props();
</script>

<div
	class="min-h-screen bg-neutral-950 font-sans text-neutral-100 selection:bg-cyan-500/30 selection:text-cyan-200"
>
	<header
		class="sticky top-0 z-40 border-b border-neutral-800/80 bg-neutral-900/50 backdrop-blur-md"
	>
		<div class="mx-auto flex h-16 max-w-5xl items-center justify-between px-6">
			<div class="flex items-center gap-2">
				<div class="h-3 w-3 rounded-full bg-cyan-400 shadow-[0_0_10px_#22d3ee]"></div>
				<span class="text-lg font-bold tracking-tight text-white"
					>DevPulse<span class="text-cyan-400">.log</span></span
				>
			</div>
			<span
				class="rounded-full border border-neutral-700/50 bg-neutral-800/80 px-2.5 py-1 text-xs text-neutral-400"
			>
				API Demo
			</span>
		</div>
	</header>

	<main class="mx-auto max-w-5xl px-6 py-10">
		{@render children()}
	</main>
</div>
