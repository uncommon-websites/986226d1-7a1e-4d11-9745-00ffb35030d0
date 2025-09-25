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
	title="Turn viral moments into verified value"
	subtitle="Coin transforms your tweets into tradeable tokens instantly. Join 55,000+ creators monetizing memes on Base blockchain with one-click deployment."
	imageSrc="/generated/image-a-young-diverse-creator-in-their-bedroom.webp"
	callsToAction={[
		{ href: "#waitlist", label: "Join waitlist" },
		{ href: "#learn-more", label: "Learn more" }
	]}
/>
<LogoScroller 
	label="Trusted by leading crypto creators and platforms" 
	logoUrls={[
		'https://cdn.brandfetch.io/farcaster.xyz/w/400/h/400/logo',
		'https://cdn.brandfetch.io/magiceden.io/w/400/h/400/logo', 
		'https://cdn.brandfetch.io/coinbase.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/x.com/w/400/h/400/logo'
	]}
/>

<Summary
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	generating
	testimonials={[
		{
			name: "Jane Smith",
			position: "CTO",
			company: "Tech Innovations",
			quote:
				"Their cutting-edge automation boosted our productivity by 35%.\nThe intuitive interface reduced training time and improved team adoption.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "John Doe",
			position: "Director of Operations",
			company: "Global Solutions",
			quote:
				"Their robust security protocols gave us confidence in handling sensitive data.\nThe 24/7 support team resolved issues within hours, not days.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Sarah Johnson",
			position: "Product Manager",
			company: "Future Systems",
			quote:
				"The scalable platform grew seamlessly with our business needs.\nTheir customization options allowed us to tailor solutions perfectly to our workflows.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<Features
	title="Turn moments into markets"
	subtitle="Built for crypto creators who know the value of viral timing"
	features={[
		{
			title: "One-click meme coin deployment",
			description: "Transform any tweet into a tradeable token instantly without complex smart contract knowledge. Skip the 80% profit loss from timing delays and capture value while your content trends.",
			imageSrc: "/generated/image-a-diverse-group-of-young-creators-in-the.webp"
		},
		{
			title: "AI-powered viral detection",
			description: "Our proprietary algorithms identify trending potential before mainstream platforms catch on. Get first-mover advantage on your most valuable content moments.",
			imageSrc: "/generated/image-a-small-diverse-group-of-creators-collab.webp"
		},
		{
			title: "Base blockchain infrastructure",
			description: "Built on Coinbase's Layer 2 for lightning-fast transactions and minimal fees. Your meme coins deploy in seconds, not minutes, keeping pace with internet speed culture.",
			imageSrc: "/generated/image-a-solo-creator-in-their-bedroom-studio-c.webp"
		},
		{
			title: "Seamless social authentication",
			description: "Connect your Twitter account with one click and start monetizing immediately. No complex wallet setups or crypto knowledge required to begin earning.",
			imageSrc: "/generated/image-a-diverse-creator-collective-brainstormi.webp"
		},
		{
			title: "Real-time market tracking",
			description: "Monitor your meme coin performance with live market cap updates and trading volume analytics. Watch your viral moments generate actual revenue in real-time.",
			imageSrc: "/generated/image-real-time-crypto-trading-dashboard-with-.webp"
		},
		{
			title: "Permanent IPFS storage",
			description: "Your meme coins and content are stored permanently on decentralized networks, ensuring your digital assets remain accessible forever. True ownership of your viral moments.",
			imageSrc: "/generated/image-decentralized-storage-network-with-glowi.webp"
		}
	]}
/>
<AboutTeaser generating />
<CallToAction generating />
