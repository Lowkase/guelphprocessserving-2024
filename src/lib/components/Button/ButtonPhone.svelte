<script>
	import phone from '$lib/svgs/phone.svg?raw';

	export let phoneNumber = '';
	export let scheme = '';
	export let svgShow = false;
	export let text = '';

	// tellLink if it exists
	$: telLink = phoneNumber ? `tel:${phoneNumber}` : '#';
</script>

<a
    class="m-button {scheme}"
    href={telLink}
    rel="noreferrer"
    target="_blank"
    aria-label={`Call ${phoneNumber}`}
>
    {#if svgShow}
        {@html phone}
    {/if}
    <div class="text">{text}</div>
</a>

<style>
    @import url('Button.css');
</style>