<script lang="ts">
	let { children, class: className = '' }: { children: any; class?: string } = $props();
</script>

<section class="py-20 md:py-28 {className}">
	<div class="max-w-3xl mx-auto px-6">
		{@render children()}
	</div>
</section>
