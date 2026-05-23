<script lang="ts">
	import Section from '$lib/components/Section.svelte';
</script>

<svelte:head>
	<title>QuantSlate — Educational Trading Engine</title>
	<meta name="description" content="QuantSlate is an educational algorithmic trading engine written in OCaml, inspired by Jane Street and Goldman Sachs SecDB." />
</svelte:head>

<!-- Hero -->
<section class="pt-24 pb-16 md:pt-40 md:pb-24 border-b border-neutral-100">
	<div class="max-w-3xl mx-auto px-6">
		<h1 class="text-5xl md:text-7xl font-bold tracking-tight text-brand-950 mb-8">
			QuantSlate
		</h1>
		<p class="text-xl md:text-2xl text-neutral-500 font-light leading-relaxed max-w-2xl">
			A research-grade algorithmic trading engine built as an educational exploration into the systems that power modern markets.
		</p>
		<div class="mt-10 flex flex-wrap gap-4">
			<a href="/architecture" class="inline-flex items-center px-5 py-3 bg-brand-950 text-white text-sm font-medium rounded-lg hover:bg-brand-900 transition-colors">
				Explore Architecture
			</a>
			<a href="/about" class="inline-flex items-center px-5 py-3 border border-neutral-300 text-neutral-700 text-sm font-medium rounded-lg hover:border-neutral-400 hover:text-brand-950 transition-colors">
				Read the Story
			</a>
		</div>
	</div>
</section>

<!-- Pillars -->
<Section>
	<div class="grid md:grid-cols-3 gap-12">
		<div>
			<div class="w-10 h-10 rounded-lg bg-neutral-100 flex items-center justify-center mb-4">
				<span class="font-mono text-sm font-bold text-brand-950">ml</span>
			</div>
			<h3 class="text-lg font-semibold text-brand-950 mb-2">Jane Street</h3>
			<p class="text-neutral-600 text-sm leading-relaxed">
				Inspired by their rigorous approach to functional programming in OCaml. Type safety, immutable data structures, and composable abstractions form the backbone of our engine.
			</p>
		</div>
		<div>
			<div class="w-10 h-10 rounded-lg bg-neutral-100 flex items-center justify-center mb-4">
				<span class="font-mono text-sm font-bold text-brand-950">db</span>
			</div>
			<h3 class="text-lg font-semibold text-brand-950 mb-2">Goldman Sachs SecDB</h3>
			<p class="text-neutral-600 text-sm leading-relaxed">
				Borrowing the philosophy of a unified securities database where instruments, prices, and risk metrics live in a single, coherent graph. Risk is a first-class citizen.
			</p>
		</div>
		<div>
			<div class="w-10 h-10 rounded-lg bg-neutral-100 flex items-center justify-center mb-4">
				<span class="font-mono text-sm font-bold text-brand-950">in</span>
			</div>
			<h3 class="text-lg font-semibold text-brand-950 mb-2">Zerodha Kite</h3>
			<p class="text-neutral-600 text-sm leading-relaxed">
				Leveraging India's most accessible retail brokerage API to bridge the gap between academic curiosity and live market data. Democratizing market access for learners.
			</p>
		</div>
	</div>
</Section>

<!-- Stack -->
<section class="py-20 md:py-28 bg-neutral-50 border-y border-neutral-100">
	<div class="max-w-3xl mx-auto px-6">
		<h2 class="text-2xl font-semibold tracking-tight text-brand-950 mb-8">Technology Stack</h2>
		<div class="grid grid-cols-2 md:grid-cols-4 gap-6">
			{#each [
				{ name: 'OCaml', desc: 'Core language' },
				{ name: 'Async', desc: 'Concurrency' },
				{ name: 'Zerodha Kite', desc: 'Market API' },
				{ name: 'PostgreSQL', desc: 'Persistence' },
				{ name: 'SvelteKit', desc: 'Web interface' },
				{ name: 'TimescaleDB', desc: 'Time-series' },
				{ name: 'Protocol Buffers', desc: 'Serialization' },
				{ name: 'Docker', desc: 'Deployment' }
			] as item}
				<div class="bg-white border border-neutral-200 rounded-lg p-4">
					<p class="font-semibold text-brand-950 text-sm">{item.name}</p>
					<p class="text-xs text-neutral-500 mt-1">{item.desc}</p>
				</div>
			{/each}
		</div>
	</div>
</section>

<!-- Disclaimer Banner -->
<section class="py-12 bg-amber-50 border-b border-amber-100">
	<div class="max-w-3xl mx-auto px-6">
		<div class="flex items-start gap-4">
			<div class="w-8 h-8 rounded-full bg-amber-100 flex items-center justify-center shrink-0 mt-0.5">
				<span class="text-amber-700 text-sm font-bold">!</span>
			</div>
			<div>
				<h3 class="text-sm font-semibold text-amber-900 mb-1">Educational Project Disclaimer</h3>
				<p class="text-sm text-amber-800 leading-relaxed">
					QuantSlate is an educational implementation intended for learning purposes only. It is not designed for production trading, nor does it constitute financial or investment advice. Trading in financial markets carries substantial risk of loss.
				</p>
				<a href="/disclaimer" class="inline-block mt-3 text-sm font-medium text-amber-900 underline underline-offset-2 hover:text-amber-950">
					Read Full Disclaimer
				</a>
			</div>
		</div>
	</div>
</section>
