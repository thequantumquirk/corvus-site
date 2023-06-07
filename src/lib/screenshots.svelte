<script>
	// @ts-nocheck
	import Carousel from 'svelte-carousel';
	import { browser } from '$app/environment';
	let carousel;
</script>

<main id="screenshots">
	<section class="py-16 bg-light-black rounded-lg">
		<div
			class="xl:mx-32 2xl:mx-64 lg:mx-16 mx-8 pb-8 flex items-center justify-end lg:text-4xl text-2xl font-bold"
		>
			Screenshots
		</div>
		<div class="w-4/6 mx-auto hidden xl:block">
			{#if browser}
				<Carousel particlesToShow={3} particlesToScroll={2} bind:this={carousel}>
					{#each { length: 14 } as _, index}
						<div class="flex justify-center">
							<img
								class="rounded-lg"
								src="https://ik.imagekit.io/corvus/corvus_{index + 1}.jpg"
								alt="Corvus"
								width="250px"
							/>
						</div>
					{/each}
				</Carousel>
			{/if}
		</div>
		<div class="w-3/4 mx-auto xl:hidden lg:block hidden">
			{#if browser}
				<Carousel particlesToShow={2} bind:this={carousel}>
					{#each { length: 14 } as _, index}
						<div class="flex justify-center">
							<img
								class="rounded-lg"
								src="https://ik.imagekit.io/corvus/corvus_{index + 1}.jpg"
								alt="Corvus"
								width="250px"
							/>
						</div>
					{/each}
				</Carousel>
			{/if}
		</div>
		<div class="w-3/4 mx-auto lg:hidden block">
			{#if browser}
				<Carousel bind:this={carousel}>
					{#each { length: 14 } as _, index}
						<div class="flex justify-center">
							<img
								class="rounded-lg"
								src="https://ik.imagekit.io/corvus/corvus_{index + 1}.jpg"
								alt="Corvus"
								width="250px"
							/>
						</div>
					{/each}
				</Carousel>
			{/if}
		</div>
	</section>
</main>
