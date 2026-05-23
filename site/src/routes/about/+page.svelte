<script lang="ts">
	import Section from '$lib/components/Section.svelte';
</script>

<svelte:head>
	<title>About — QuantSlate</title>
	<meta name="description" content="Learn about the QuantSlate project, its educational mission, and the inspirations behind it." />
</svelte:head>

<Section class="prose-custom">
	<h1>About the Project</h1>

	<p class="text-lg text-neutral-600 leading-relaxed">
		QuantSlate was born from a simple question: <em>How do the world's most sophisticated financial institutions think about software?</em> 
		This project is a ground-up educational reconstruction of the architectural patterns that drive high-performance trading systems.
	</p>

	<h2>Mission</h2>
	<p>
		Our goal is to demystify the technology behind quantitative trading and market infrastructure. By building an engine from scratch, 
		we explore the intersection of functional programming, systems design, and financial markets — without the pressure of production capital at risk.
	</p>

	<h2>Why OCaml?</h2>
	<p>
		OCaml offers a rare combination of expressiveness, type safety, and runtime performance. Its powerful type system catches entire classes 
		of bugs at compile time, while its pattern matching and module system make domain modeling exceptionally clear. 
		These properties have made it the language of choice at firms like Jane Street, where correctness under uncertainty is paramount.
	</p>

	<h2>Why SecDB?</h2>
	<p>
		Goldman Sachs' SecDB represents a paradigm where securities are not just rows in a database, but nodes in a unified computational graph. 
		Every instrument knows its dependencies, every price change propagates through the graph, and risk is computed continuously rather than periodically. 
		We adopt this philosophy to build a coherent, queryable model of the market.
	</p>

	<h2>Why Zerodha Kite?</h2>
	<p>
		India's capital markets are deep, vibrant, and increasingly accessible. Zerodha's Kite Connect API provides a well-documented, 
		modern interface to live market data and order execution. It allows us to ground our theoretical engine in real-world 
		market semantics — from NSE equities to F&O contracts — while remaining firmly in the educational domain.
	</p>

	<h2>An Educational Endeavour</h2>
	<p>
		Every line of code in QuantSlate is written to be read, understood, and critiqued. We prioritize clarity over cleverness, 
		and correctness over speed. The project is open for inspection, discussion, and learning. We believe that the best way to understand 
		complex systems is to rebuild them — carefully, thoughtfully, and transparently.
	</p>

	<div class="mt-12 p-6 bg-neutral-50 rounded-lg border border-neutral-200">
		<p class="text-sm text-neutral-600 mb-0">
			<strong>Note:</strong> QuantSlate does not execute live trades. Any integration with brokerage APIs is strictly for data ingestion 
			and simulated (paper) trading. No real money is ever at stake.
		</p>
	</div>
</Section>
