<script>
	import ButtonPhone from '$lib/components/ButtonPhone.svelte'
	import logo from '$lib/svgs/logo.svg?raw';
</script>

<header>
	<a class="logo" href="/" aria-label="Home">
		{@html logo}
		<span>Mike Vecchio RMT</span>
	</a>

	<div class="links">
		<ButtonPhone
			phoneNumber="519-859-1419"
			scheme="m-button-header m-button-collapse-mobile"
			svgShow={true}
			text="519-859-1419"
		/>
	</div>
</header>