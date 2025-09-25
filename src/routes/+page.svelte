<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CenteredTextOnlyHero from "$lib/components/layout/hero-sections/CenteredTextOnlyHero.svelte";
</script>

<CenteredTextOnlyHero
	title="Turn tweets into tradeable assets"
	subtitle="Coin delivers instant meme monetization by converting viral social content into blockchain tokens with AI-powered analysis."
	imageSrc="/generated/image-a-young-diverse-creator-in-their-lived-i.webp"
/>
<LogoScroller
	label="Trusted by crypto innovators and creator platforms"
	logoUrls={[
		'https://cdn.brandfetch.io/coinbase.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/x.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/opensea.io/w/400/h/400/logo',
		'https://cdn.brandfetch.io/discord.com/w/400/h/400/logo'
	]}
/>

<Summary
	title="Turn viral moments into value"
	text="Coin lets meme creators and crypto influencers instantly mint tokens from their most viral tweets. No devs, no tokenomics — just one click and your content becomes a tradeable market. Every viral post is a missed opportunity until now."
/>

<Testimonials
	testimonials={[
		{
			name: "Marcus Thompson",
			position: "Crypto Influencer",
			company: "45K Twitter Followers",
			quote:
				"Coin saved me 18 hours per week by automating token creation from my viral tweets.\nI've generated $12K in revenue from memes that would have just disappeared into the timeline.",
			image: "/generated/image-medium-shot-portrait-of-a-confident-youn.webp"
		},
		{
			name: "Zara Chen",
			position: "Meme Creator",
			company: "78K Social Media Following",
			quote:
				"Used to miss 80% of monetization opportunities from trending posts - now I capture them instantly.\nThe one-click token deployment turned my best meme into $8,500 in trading volume within 6 hours.",
			image: "/generated/image-medium-shot-portrait-of-a-confident-asia.webp"
		},
		{
			name: "Diego Morales",
			position: "Content Creator",
			company: "32K Farcaster Network",
			quote:
				"Coin eliminated the $2,000 upfront cost and 3-week learning curve for token launches.\nMy first meme coin hit $15K market cap while the content was still trending - perfect timing that was impossible before.",
			image: "/generated/image-medium-shot-portrait-of-a-confident-lati.webp"
		}
	]}
/>

<Features
	title="Turn viral moments into valuable assets"
	subtitle="Transform your tweets into tradeable tokens instantly with AI-powered meme monetization"
	features={[
		{
			title: "One-click meme monetization",
			description:
				"Convert any viral tweet into a tradeable token without complex blockchain knowledge. Simply connect your Twitter account and watch your memes become markets."
		},
		{
			title: "AI-powered viral detection",
			description:
				"Our intelligent algorithms identify trending content before it peaks, ensuring you capture maximum value from your creative moments."
		},
		{
			title: "Instant tweet-to-token conversion",
			description:
				"Deploy your meme coin on Base Protocol in seconds, not hours. Don't miss the wave while others struggle with technical barriers."
		},
		{
			title: "Built on Base Protocol",
			description:
				"Leverage Coinbase's secure Layer 2 solution for fast, low-cost transactions. Your tokens benefit from enterprise-grade blockchain infrastructure."
		},
		{
			title: "Creator attribution and royalties",
			description:
				"Maintain ownership of your creative work while earning ongoing royalties. Every trade generates value back to the original creator."
		},
		{
			title: "Seamless social integration",
			description:
				"Connect Twitter, authenticate with Privy wallet, and mint tokens directly from your social media dashboard. No technical setup required."
		}
	]}
/>
<AboutTeaser />
<CallToAction />
