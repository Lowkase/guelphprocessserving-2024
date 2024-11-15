<script>
	import Image404 from '$lib/images/404.jpg'

	import Header from '$lib/components/Header.svelte'
	import Footer from '$lib/components/Footer.svelte'
</script>

<Header />
<main class="p-404">
	<section>
		<img class="image-404" src={Image404} alt="You can't get there from here" />
		<div class="notfound">
			404: Page not found
		</div>
		<div>
			You can't get there from here.<br/>Click <a href="/">here</a> to get back to civilization.
		</div>
	</section>
</main>
<Footer />

<style>
	.p-404 {
		text-align: center;
	}

	.image-404 {
		margin-bottom: var(--spacing-20);
		width: 300px;
	}
	.notfound {
		font-size: var(--font-size-m);
		font-weight: bold;
		margin-bottom: var(--spacing-8);
	}
</style>