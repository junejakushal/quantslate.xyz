<script lang="ts">
	import Section from '$lib/components/Section.svelte';
</script>

<svelte:head>
	<title>Disclaimer — QuantSlate</title>
	<meta name="description" content="QuantSlate disclaimer and legal notices." />
</svelte:head>

<Section class="prose-custom">
	<h1>Disclaimer</h1>

	<div class="p-6 bg-red-50 border border-red-100 rounded-lg mb-10">
		<p class="text-red-900 font-semibold mb-2">Not Financial Advice</p>
		<p class="text-red-800 text-sm leading-relaxed mb-0">
			QuantSlate is an educational and research project. Nothing on this website or in the associated source code 
			constitutes financial advice, investment recommendations, or an offer to buy or sell any financial instrument.
		</p>
	</div>

	<h2>Educational Purpose Only</h2>
	<p>
		This project is designed solely for learning about software architecture, functional programming, and market technology. 
		It is not intended for production use, live trading, or the management of real capital. The authors assume no responsibility 
		for any actions taken by third parties based on the information or code provided here.
	</p>

	<h2>No Warranties</h2>
	<p>
		The software and documentation are provided "as is", without warranty of any kind, express or implied, including but not limited 
		to the warranties of merchantability, fitness for a particular purpose, and noninfringement. In no event shall the authors 
		be liable for any claim, damages, or other liability, whether in an action of contract, tort, or otherwise, arising from, 
		out of, or in connection with the software or the use or other dealings in the software.
	</p>

	<h2>Trading Risks</h2>
	<p>
		Trading in financial markets involves substantial risk of loss and is not suitable for all individuals. Past performance, 
		whether real or simulated, is not indicative of future results. You should carefully consider whether trading is appropriate 
		for you in light of your experience, objectives, and financial resources.
	</p>

	<h2>Third-Party APIs</h2>
	<p>
		QuantSlate may reference or demonstrate integration with third-party APIs, including but not limited to Zerodha Kite Connect. 
		Use of these APIs is subject to their respective terms of service. This project is not affiliated with, endorsed by, or sponsored 
		by Zerodha, Jane Street, Goldman Sachs, or any other mentioned entity.
	</p>

	<h2>Open Source & Attribution</h2>
	<p>
		Code and concepts may be inspired by publicly available research, whitepapers, and industry practice. All trademarks and registered 
		trademarks are the property of their respective owners. Any mention of specific firms or products is for contextual and educational 
		illustration only.
	</p>

	<p class="text-sm text-neutral-500 mt-12">
		Last updated: May 2026
	</p>
</Section>
