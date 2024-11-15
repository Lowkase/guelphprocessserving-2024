<script>
	import hero from '$lib/images/hero.jpg'
	import calendar from '$lib/svgs/calendar.svg?raw';

    import ButtonLink from '$lib/components/ButtonLink.svelte'
</script>

<div class="m-hero">
	<div class="image-con">
		<img class="image" src={hero} alt="Treatment Room" />
	</div>
	<div class="mask"></div>
	<div class="content">
		<div>
			<h1 class="message">Massage therapy in a relaxing environment</h1>
			<ButtonLink
				link="https://mikevecchiormt.clinicsense.com/book"
				scheme="m-button-content"
				svgShow={true}
				svgSvg={calendar}
				text="BOOK AN APPOINTMENT"
			/>
		</div>
	</div>
</div>