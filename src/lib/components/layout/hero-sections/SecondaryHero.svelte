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

<header class="relative overflow-hidden bg-black" {...rest}>
	<!-- Background gradient overlay -->
	<div class="absolute inset-0 bg-gradient-to-br from-purple-900/20 via-black to-cyan-900/20"></div>
	
	<!-- Subtle grid pattern -->
	<div class="absolute inset-0 opacity-10" style="background-image: radial-gradient(circle at 1px 1px, rgb(255,255,255) 1px, transparent 0); background-size: 40px 40px;"></div>
	
	<div class="relative section-px section-py container mx-auto">
		<div class="grid gap-12 lg:grid-cols-2 lg:gap-16 items-center">
			<!-- Content Section -->
			<div class="order-2 lg:order-1">
				<div class="space-y-6">
					<h1 class="text-display font-bold text-white">
						<span class="block">{title}</span>
					</h1>
					<p class="text-callout text-gray-300 leading-relaxed max-w-lg">
						{subtitle}
					</p>
					
					<!-- Accent highlight -->
					<div class="h-px w-20 bg-gradient-to-r from-cyan-400 to-purple-500"></div>
				</div>
			</div>
			
			<!-- Image Section -->
			<div class="order-1 lg:order-2">
				<div class="relative group">
					<!-- Neon glow effect -->
					<div class="absolute -inset-1 bg-gradient-to-r from-cyan-400/20 to-purple-500/20 rounded-xl blur opacity-75 group-hover:opacity-100 transition duration-1000"></div>
					
					<div class="relative aspect-video overflow-hidden rounded-xl bg-gray-900 border border-gray-800">
						<img
							class="h-full w-full object-cover transition-transform duration-500 group-hover:scale-105"
							src={imageSrc}
							alt="Coin team collaborating on meme monetization platform"
						/>
						
						<!-- Overlay gradient -->
						<div class="absolute inset-0 bg-gradient-to-t from-black/30 via-transparent to-transparent"></div>
					</div>
				</div>
			</div>
		</div>
	</div>
</header>
