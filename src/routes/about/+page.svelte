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
    title: "Practical solutions",
    description: "We build tools that actually help small businesses run smoother. No jargon, no fluff—just things that work."
  },
  {
    title: "Everyday collaboration",
    description: "We know small business means teamwork. We work closely with each other, and with our users, to get real results."
  },
  {
    title: "People first",
    description: "Whether serving customers or supporting teammates, we care about people. We listen, respect, and keep things simple."
  },
  {
    title: "Transparency always",
    description: "We keep communication open and honest—inside our team, and with every business that trusts us."  
  },
  {
    title: "Keep it accessible",
    description: "Small businesses move fast and do it all themselves. We make our app easy to learn, with support when it matters most."
  }
];
</script>

<SecondaryHero
	title="Run your business from anywhere"
	subtitle="Everything you need to sell, ship, and manage—right from your phone"
	imageSrc="/generated/image-a-small-business-team-collaborating-in-a.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Running a small business is tough. Too often, you're buried under inventory guesses, last-minute customer updates, or scrambling to find the right notebook or app just to track a sale. You're doing the work of five people—with tools built for big companies, not small ones like yours.",
		"Commerce Systems started because we lived that frustration. One of our founders ran a small grocery shop with their family, juggling handwritten orders, mismatched spreadsheets, and constant texts from vendors and staff. They didn’t need a complicated dashboard—they just needed something simple that worked, wherever they were.",
		"We believe small business software should feel as easy as texting a friend. So we built an app that brings together the most important parts of your business—products, orders, and customers—all in your pocket. No clutter, no fluff. Just the basics done right, so you can get back to actually running your business."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Meet our founder."
	subtitle="Commerce Systems grew out of real small business experience. One of our founders ran a grocery shop with their family, juggling handwritten orders, mismatched notes, and constant text updates. Today, that hands-on experience shapes every decision we make."
	stakeholders={[
		{
			name: "Commerce Systems Founder",
			position: "Founder",
			bio: "A small business owner who built Commerce Systems after feeling the daily frustrations of running a family grocery shop. Solutions here are shaped by real world needs—never corporate guesswork.",
			image: "/generated/image-a-friendly-business-founder-poses-for-a-.webp"
		}
	]}
/>

<!-- No investors to show -->

<!-- CTA Section -->
<CallToAction
  title="Let’s make commerce simpler."
  subtitle="See how Commerce Systems fits your business."
  description="Ready to spend less time on operations and more time serving your customers? Try the app, reach out with questions, or join the team that cares about real-world results."
  imageSrc="/generated/image-a-friendly-small-business-owner-with-a-w.webp"
  callsToAction={[
    { href: "/signup", label: "Try it free", variant: "primary" },
    { href: "/contact", label: "Get in touch", variant: "secondary" },
    { href: "/careers", label: "Join our team", variant: "secondary" }
  ]}
/>
