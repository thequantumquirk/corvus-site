<script>
	// @ts-nocheck
	import Screenshots from '$lib/screenshots.svelte';
	import Specials from '$lib/specials.svelte';
	import Team from '$lib/team.svelte';
	let pageTitle = 'Corvus AOSP | GET THE RAVEN UNLEASHED';
	let pageDescription =
		'Experience the power of Corvus AOSP Custom ROM - a feature-packed Android ROM designed for optimal performance and customization. Unlock a new level of smartphone personalization.';
</script>

<svelte:head>
	<title>{pageTitle}</title>
	<meta name="description" content={pageDescription} />
	<meta property="og:title" content={pageTitle} />
	<meta property="og:description" content={pageDescription} />
	<meta property="og:image" content="https://ik.imagekit.io/corvus/corvus.jpg" />
	<meta property="og:url" content="https://www.corvusrom.com" />
</svelte:head>

<main id="hero" class="w-screen lg:pt-56 pt-36">
	<div class="flex item-center gap-2 md:justify-around justify-between">
		<img
			class="block md:hidden"
			src="https://ik.imagekit.io/corvus/crow2.png?tr=w-130&ik-sdk-version=javascript-1.4.3&updatedAt=1677731135645"
			alt="Corvus"
		/>
		<div class="mx-2">
			<h1 class="lg:text-7xl text-3xl font-extrabold">GET THE RAVEN <br />UNLEASHED</h1>
			<p class="lg:text-2xl text-primary font-medium lg:my-8 my-2">The Experience You Deserve</p>
			<!-- <a href="/devices"
				><button class="bg-primary lg:text-base text-sm p-2 m-1 rounded-lg font-bold"
					>Download Now!</button
				></a
			>
			<button
				class="lg:text-base text-sm border border-light-primary text-light-primary m-1 py-2 px-5 rounded-lg font-bold"
				>What's New</button
			> -->
			<p
				class="text-light-primary font-bold lg:text-2xl rounded-lg border-light-primary border p-2 text-center"
			>
				We'll be back on track soon!
			</p>
		</div>
		<img
			class="hidden md:block"
			src="https://ik.imagekit.io/corvus/crow.png?tr=w-400&ik-sdk-version=javascript-1.4.3&updatedAt=1677226946997"
			alt="Corvus"
		/>
	</div>
	<Specials />
	<Team />
	<Screenshots />
</main>
