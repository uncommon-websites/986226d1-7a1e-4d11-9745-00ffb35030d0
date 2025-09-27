<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Creators first",
			description: "Every viral moment deserves instant monetization. We put meme creators at the center of their own economic opportunity."
		},
		{
			title: "Culture follows value",
			description: "The most valuable content emerges from authentic culture. We turn cultural moments into tradeable assets with one click."
		},
		{
			title: "Speed of memes",
			description: "Viral windows close fast. Our AI-powered deployment gets your meme coin live before the moment passes."
		}
	];
</script>

<SecondaryHero
	title="Make memes. Mint money."
	subtitle="Instant value from viral content"
	imageSrc="/generated/image-a-diverse-group-of-young-adults-dressed-.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Coin was born out of a frustration shared by every viral meme creator: you're making culture, but you're not making money. Tweets catch fire, memes take off, and the value flows—everywhere except your wallet. Our team saw creators missing 80% of the upside from social virality, simply because there was no easy way to monetize the moment. We asked a simple question: what if every viral post came with its own economy?",
		"That question led us to build Coin—an AI-powered platform that turns your most viral content into tradeable meme coins with one click. We handle the complexity behind the scenes: smart contract deployment, Base blockchain integration, Twitter authentication, IPFS image storage, and wallet onboarding. All you do is connect your account, select a viral tweet, and click. From there, it's instantly live—minted, listed, and ready to trade.",
		"Now, our mission is simple: to give creators instant ownership over the value they generate online. We're building a new layer of the internet, one where memes have markets and attention turns into real value. The early web rewarded engagement. The new web rewards economics. If you've got an audience and a viral post, Coin gives you the tools to capture the upside—before it scrolls away."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	generating
	stakeholderType="team"
	title="Our team."
	subtitle="Your partners in innovation."
	stakeholders={[
		{
			name: "Alex Morgan",
			position: "Founder & CEO",
			bio: "Started the company with a vision to transform the industry through innovative solutions.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Jamie Chen",
			position: "Chief Design Officer",
			bio: "Award-winning designer with a passion for creating intuitive and beautiful experiences.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Taylor Wright",
			position: "Head of Engineering",
			bio: "Technology enthusiast focused on building scalable systems that make a difference.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<StakeholderGrid
	generating
	stakeholderType="investor"
	title="Backed by the best."
	subtitle="Point Nine, TSIC and others"
	stakeholders={[
		{
			name: "Point Nine Capital",
			image: "https://cdn.brandfetch.io/pointnine.com/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7"
		},
		{
			name: "TSIC Ventures",
			image: "https://cdn.brandfetch.io/tiny.vc/w/400/h/400/logo?c=1a2b3c4d5e"
		},
		{
			name: "Sequoia Capital",
			image: "https://cdn.brandfetch.io/sequoiacap.com/w/400/h/400/logo"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Turn your memes into money."
	subtitle="Join the meme monetization revolution"
	description="Join 55,000+ creators already on our waitlist. Start capturing the upside from your viral content—before it scrolls away."
	imageSrc="/generated/image-a-young-diverse-creator-in-their-persona.webp"
	callsToAction={[
		{
			href: "#waitlist",
			label: "Join waitlist",
			variant: "primary"
		},
		{
			href: "#demo",
			label: "See demo",
			variant: "secondary"
		}
	]}
/>
