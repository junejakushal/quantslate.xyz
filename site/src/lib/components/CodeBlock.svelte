<script lang="ts">
	let { code, language = 'ocaml' }: { code: string; language?: string } = $props();
</script>

<div class="my-6 rounded-lg overflow-hidden bg-brand-950">
	<div class="flex items-center justify-between px-4 py-2 bg-brand-900 border-b border-white/10">
		<span class="text-xs font-medium text-neutral-400 uppercase tracking-wider">{language}</span>
	</div>
	<pre class="p-4 overflow-x-auto text-sm leading-relaxed text-neutral-300 font-mono"><code>{code}</code></pre>
</div>
