<script>
	import hero from '$lib/images/hero.jpg'
	import Logo from '$lib/svgs/logo.svg?raw';
	
    import ButtonEmail from '$lib/components/ButtonEmail.svelte'
	import ButtonPhone from '$lib/components/ButtonPhone.svelte'
</script>

<div class="m-hero">
	<div class="image-con">
		<img class="image" src={hero} alt="Legal documents being served" />
	</div>
	<div class="mask"></div>
	<div class="content">
		<div class="logo">
			{@html Logo}
		</div>
		<div class="text">
			<h1 class="title">
				Guelph Process Serving & Court Filing
			</h1>
			<p class="description">
				Efficient document handeling for <strong>Guelph Ontario</strong> and surrounding areas
			</p>
		</div>
		<div class="actions">
			<ButtonEmail
				emailAddress= "guelphprocessserving@rogers.com"
				emailSubject="Requesting Information"
				scheme="m-button-header"
				svgShow={true}
				text="Email Us"
			/>
			<ButtonPhone
				phoneNumber="519-400-1479"
				scheme="m-button-header"
				svgShow={true}
				text="519-400-1479"
			/>
		</div>
	</div>
</div>