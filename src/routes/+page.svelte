<script lang="ts">
	// Components
	import UseCases from "$lib/components/layout/UseCases.svelte";
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";
</script>

<CustomerCardHero
  centered={true}
  title="Run your business from your phone"
  subtitle="hi"
  customers={[
    {
      name: "Lucy Nguyen",
      position: "Owner, Lucy's Flower House",
      imageSrc: "/generated/image-a-female-small-business-owner-smiling-wa.webp"
    },
    {
      name: "James Patel",
      position: "Chef & Owner, Golden Table Bistro",
      imageSrc: "/generated/image-a-male-restaurant-owner-standing-confide.webp"
    },
    {
      name: "Maria Lopez",
      position: "Baker, La Dulce Vida",
      imageSrc: "/generated/image-a-middle-aged-woman-behind-the-counter-o.webp"
    },
    {
      name: "Tom O'Reilly",
      position: "Owner, O'Reilly Hardware",
      imageSrc: "/generated/image-a-male-hardware-store-owner-in-a-work-ap.webp"
    },
    {
      name: "Ava Carter",
      position: "Manager, Brew Crew Café",
      imageSrc: "/generated/image-a-female-caf-manager-standing-cheerfully.webp"
    }
  ]}
/>
<LogoScroller
	label="Trusted by industry leaders"
	logoUrls={[
		'https://logo.clearbit.com/shopify.com',
		'https://logo.clearbit.com/squareup.com',
		'https://logo.clearbit.com/etsy.com',
		'https://logo.clearbit.com/bigcommerce.com'
	]}
/>

<Summary
  title="What we do"
  text="Commerce Systems helps small businesses manage sales, orders, and inventory from their phone. Our mobile app puts essential commerce tools in one place, so you can stay organized and in control—wherever you work."
/>

<Testimonials
	testimonials={[
		{
			name: "Lina Worthington",
			position: "Manager",
			company: "Little Bloom Flower Shop",
			quote: "We used to manually track inventory with notebooks—it took forever and mistakes were constant. With Commerce Systems, we saved at least 5 hours a week and stopped running out of bestseller items.",
			image: "/generated/image-a-woman-in-a-flower-shop-surrounded-by-a.webp"
		},
		{
			name: "Raul Crespo",
			position: "Owner",
			company: "Panaderia Crespo",
			quote: "Before, we missed online orders and had no clear system. Now every transaction is logged, and errors dropped by 80%. Commerce Systems gave us the visibility we needed.",
			image: "/generated/image-a-man-behind-a-bakery-counter-rolling-do.webp"
		},
		{
			name: "Dana Bhuiyan",
			position: "Co-founder",
			company: "Canvas Studio & Supply",
			quote: "Switching to Commerce Systems cut our payment processing fees by 20% and eliminated the need for extra POS hardware. The money we save goes straight back into the business.",
			image: "/generated/image-a-woman-in-an-arts-and-crafts-store-orga.webp"
		}
	]}
/>

<Features
	title="Do more with less busywork"
	subtitle="The essential tools for small business commerce, all in one place."
	features={[
		{
			title: "Easy order management",
			description: "Create and track orders in seconds, no paperwork required."
		},
		{
			title: "Inventory tracking",
			description: "Monitor stock levels in real time and avoid running out."
		},
		{
			title: "Payment processing",
			description: "Accept card and contactless payments without extra hardware."
		},
		{
			title: "Customer database",
			description: "Keep customer details and purchase histories organized."
		},
		{
			title: "On-the-go access",
			description: "Manage your business from anywhere—shop, home, or the road."
		},
		{
			title: "Real-time reporting",
			description: "View sales and performance insights whenever you need them."
		}
	]}
/>

<UseCases
	title="Use Cases"
	subtitle="Real-world applications for your business needs"
	useCases={[
		{
			title: "Simplify supplier reordering",
			description: "Set automated restock alerts, send purchase orders, and track deliveries—without the back-and-forth emails.",
			image: "/generated/image-a-small-business-owner-is-joyfully-organ.webp",
			link: {
				href: "/use-cases/supplier-management",
				label: "Learn more"
			}
		},
		{
			title: "Automate local delivery coordination",
			description: "Keep track of drop-offs, notify buyers, and route drivers—in just a few taps.",
			image: "/generated/image-a-friendly-courier-is-delivering-package.webp",
			link: {
				href: "/use-cases/local-delivery-coordination",
				label: "Learn more"
			}
		},
		{
			title: "Launch customer loyalty rewards",
			description: "Reward repeat customers with points, perks, and easy redemption—no punch cards required.",
			image: "/generated/image-in-a-cozy-shop-with-rustic-wooden-interi.webp",
			link: {
				href: "/use-cases/customer-loyalty",
				label: "Learn more"
			}
		}
	]}
/>

<AboutTeaser />
<CallToAction
  title="Take control of your business"
  subtitle="Start saving hours every week—try Commerce Systems for free."
  description="Our mobile app puts all your sales, inventory, and order tools in one place—so you can streamline operations and focus on what matters. No training, no hassle."
  imageSrc="/generated/image-a-cheerful-small-business-owner-standing.webp"
  callsToAction={[
    { href: '/get-started', label: 'Start free trial', variant: 'primary' },
    { href: '/learn-more', label: 'Learn more', variant: 'secondary' }
  ]}
/>
