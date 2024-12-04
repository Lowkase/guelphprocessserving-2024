<script>
	import Email from '$lib/svgs/email.svg?raw';

	export let emailAddress = '';
	export let emailSubject = '';
	export let scheme = '';
	export let svgShow = false;
	export let text = '';
  
	let mailtoLink = "mailto:" + emailAddress + "?subject=" + emailSubject;
</script>
	
<a
	class="m-button {scheme}"
	href={mailtoLink}
	rel="noreferrer"
	target="_blank"
>
	{#if svgShow}
		{@html Email}
	{/if}
	<div class="text">{text}</div>
</a>

<style>
    @import url('Button.css');
</style>