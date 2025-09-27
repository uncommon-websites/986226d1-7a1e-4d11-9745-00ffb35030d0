<script lang="ts">
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";

	let {
		title,
		subtitle,
		imageSrc = "https://www.unc.mn/image-placeholder.svg",
		...rest
	}: {
		title: string;
		subtitle: string;
		imageSrc: string;
		[key: string]: any;
	} = $props();
</script>

<header class="bg-black text-white relative overflow-hidden" {...rest}>
	<div class="section-px section-py container mx-auto grid gap-16">
		<!-- Neon gradient overlay for brand aesthetic -->
		<div class="absolute inset-0 bg-gradient-to-br from-primary-600/20 via-transparent to-secondary-600/20 pointer-events-none"></div>
		
		<div class="relative z-10">
			<div class="section-pb-sm container-sm grid text-balance text-display text-white">
				<h2 class="font-display">
					{title}
				</h2>
				<p class="text-white/80 text-title2">
					{subtitle}
				</p>
			</div>
		</div>
		
		<div class="aspect-video overflow-clip rounded-xl bg-gray-900 border border-primary-600/30 relative z-10">
			<img
				class="h-full w-full object-cover"
				src={imageSrc}
				alt="Creative team collaborating in modern workspace"
			/>
		</div>
	</div>
</header>
