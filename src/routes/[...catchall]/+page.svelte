<script>
	import Footer from '$lib/components/Footer.svelte'
	import Hero from '$lib/components/Hero.svelte'
</script>

<Hero />
<main class="p-404">
	<section>
		<div class="notfound">
			404: Page not found
		</div>
		<div>
			Wrong page.<br/>Click <a href="/">here</a> to get back to Guelph Process Serving & Court Filing.
		</div>
	</section>
</main>
<Footer />

<style>
	.p-404 {
		text-align: center;
		margin: var(--spacing-80);
	}

	.notfound {
		font-size: var(--font-size-m);
		font-weight: bold;
		margin-bottom: var(--spacing-8);
	}
</style>