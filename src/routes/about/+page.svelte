<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Meme-first mindset",
			description: "We live and breathe internet culture. Every feature we build starts with understanding how creators actually create and what makes content go viral."
		},
		{
			title: "Speed of culture",
			description: "Viral moments move at internet speed. Our platform is built to capture value in real-time because memes wait for no one."
		},
		{
			title: "Creator sovereignty",
			description: "Creators should own their cultural impact. We exist to put financial power back in the hands of the people making the internet more interesting."
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

<!-- CTA Section -->
<CallToAction
	title="Ready to get paid to meme?"
	subtitle="Your viral moments deserve real value"
	description="Stop watching others profit from your culture. Join 55,000+ creators already on the waitlist who are ready to turn their tweets into tokens and their memes into markets. When you go viral, you should go profitable."
/>
