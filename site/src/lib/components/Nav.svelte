<script lang="ts">
	import { page } from '$app/state';

	const links = [
		{ href: '/', label: 'Home' },
		{ href: '/about', label: 'About' },
		{ href: '/architecture', label: 'Architecture' },
		{ href: '/disclaimer', label: 'Disclaimer' }
	];
</script>

<nav class="border-b border-neutral-200 bg-white/80 backdrop-blur-sm sticky top-0 z-50">
	<div class="max-w-5xl mx-auto px-6 h-16 flex items-center justify-between">
		<a href="/" class="text-lg font-bold tracking-tight text-brand-950">QuantSlate</a>
		<div class="hidden md:flex gap-8">
			{#each links as link}
				<a
					href={link.href}
					class="text-sm font-medium transition-colors {page.url.pathname === link.href
						? 'text-brand-950'
						: 'text-neutral-500 hover:text-brand-950'}"
				>
					{link.label}
				</a>
			{/each}
		</div>
	</div>
</nav>
