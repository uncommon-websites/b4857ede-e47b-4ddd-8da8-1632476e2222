<script lang="ts">
	// Types
	import type { PageProps } from "./$types";

	// Components
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import Pricing from "$lib/components/layout/Pricing.svelte";

	// Props
	const { data }: PageProps = $props();
</script>

<Pricing />

<Testimonials
  testimonials={[
    {
      name: "Jalen Avery",
      position: "Co-owner",
      company: "The Book Nook",
      quote:
        "I was skeptical about the cost at first, but Commerce Systems paid for itself in the first month. I’ve cut down administrative work by at least 10 hours a week.",
      image:
        "/generated/image-a-professional-headshot-of-an-african-am.webp"
    },
    {
      name: "Meena Kale",
      position: "General Manager",
      company: "Plants & Paper",
      quote:
        "Saving time is saving money for a shop like ours. With Commerce Systems, I can manage inventory and restock in five minutes — without calling anyone or hopping between tools.",
      image:
        "/generated/image-a-professional-headshot-of-a-south-asian.webp"
    },
    {
      name: "Tomas Rivera",
      position: "Owner",
      company: "Hilo Hardware Supply",
      quote:
        "I trust Commerce Systems with my business data completely. It's reliable, secure, and keeps everything running — even on our busiest days.",
      image:
        "/generated/image-a-professional-headshot-of-a-latino-man-.webp"
    }
  ]}
/>

<CallToAction
  title="Run your business. Not just your to-do list."
  subtitle="Spend less time juggling. Do more of what matters."
  description="Commerce Systems puts sales, inventory, and customer management in one app. Get up and running in minutes, save time every day, and keep your business moving."
  imageSrc="/generated/image-a-cheerful-small-business-owner-standing.webp"
  callsToAction={[
    { href: '/signup', label: 'Start free trial', variant: 'primary' },
    { href: '/contact', label: 'Talk to us', variant: 'secondary' }
  ]}
/>
