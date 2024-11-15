<script>
    import ButtonPhone from '$lib/components/ButtonPhone.svelte'

    const currentYear = new Date().getFullYear();
</script>

<footer>
    <div class="links">
        <ButtonPhone
            phoneNumber="519-859-1419"
            scheme="m-button-header"
            svgShow={true}
            text="519-859-1419"
        />
    </div>
    <div class="fine-print">
        <div class="copyright">©{currentYear}, Mike Vecchio RMT</div>
        <div class="rights">All rights reserved</div>
    </div>
</footer>