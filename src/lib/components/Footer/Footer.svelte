<script>
    import ButtonEmail from '$lib/components/Button/ButtonEmail.svelte'
	import ButtonPhone from '$lib/components/Button/ButtonPhone.svelte'

    const currentYear = new Date().getFullYear();
</script>

<footer>
    <div class="links">
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
    <div class="address">
        13 Robertson Dr., Guelph, ON, N1H 4S8
    </div>
    <div class="fine-print">
        <div class="copyright">©{currentYear}, Guelph Process Serving</div>
        <div class="rights">All rights reserved</div>
    </div>
</footer>

<style>
    @import url('Footer.css');
</style>