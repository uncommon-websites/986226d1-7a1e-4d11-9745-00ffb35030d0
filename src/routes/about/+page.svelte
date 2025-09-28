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
			title: "Innovation",
			description: "Constantly challenging the status quo to create better solutions."
		},
		{
			title: "Integrity",
			description: "Building trust through transparent actions and honest communication."
		},
		{
			title: "Impact",
			description: "Measuring our success by the positive change we create for our clients."
		}
	];
</script>

<SecondaryHero
	title="Get paid to go viral"
	subtitle="We exist because creators deserve to capture the value they create. When your meme breaks the internet, you should break the bank."
	imageSrc="/generated/image-a-diverse-group-of-young-creators-and-de.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Most creators miss the window. Viral moments explode across Twitter, TikTok, and beyond—generating millions of views and cultural impact—but creators watch 80% of the profit potential slip away while they scramble with complex tokenomics and blockchain mechanics. The attention economy is worth $240 billion, yet monetization remains broken for the people actually creating the culture.",
		"Coin was built to solve this disconnect. We realized that if attention is the new economy, viral moments should have real-time financial value. Our AI-powered platform analyzes your social content and converts it into tradeable meme coins instantly—no coding, no tokenomics knowledge, no waiting. Built on Base Protocol with seamless Twitter integration, we've made it as simple as turning a tweet into a token.",
		"We're democratizing the creator economy by transforming viral culture into verifiable digital assets. Every meme becomes a market. Every viral moment becomes an opportunity. For the 55,000+ creators already on our waitlist, Coin represents more than just monetization—it's about getting paid to meme and bridging the gap between cultural impact and financial opportunity in real-time."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
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
	title="Ready to coin your next viral moment?"
	subtitle="Join the meme monetization revolution"
	description="Turn your tweets into tokens and your memes into markets. Join 55,000+ creators who are already transforming viral moments into valuable digital assets."
/>
