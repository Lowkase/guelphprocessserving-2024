<script>
    export let link = '';
    export let scheme = '';
    export let svgShow = false;
    export let svgSvg = '';
    export let text = '';
</script>

<a
    class="m-button {scheme}"
    href={link}
    target="_blank"
    rel="noreferrer"
>
    {#if svgShow}
        {@html svgSvg}
    {/if}
    <div class="text">{text}</div>
</a>

<style>
    @import url('Button.css');
</style>