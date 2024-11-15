<script>
	import phone from '$lib/svgs/phone.svg?raw';

	export let emailAddress = '';
	export let emailSubject = '';
	export let emailBody = '';
	export let scheme = '';
	export let svgShow = false;
	export let text = '';
  
	// maillink if it exists
	$: mailtoLink = emailAddress
  	? `mailto:${emailAddress}?subject=${encodeURIComponent(emailSubject)}&body=${encodeURIComponent(emailBody)}`
  	:'#';</script>
  
<a
	class="m-button {scheme}"
	href={mailtoLink}
	rel="noreferrer"
	target="_blank"
>
	{#if svgShow}
		{@html phone}
	{/if}
	<div class="text">{text}</div>
</a>