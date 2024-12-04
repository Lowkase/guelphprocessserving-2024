<script>
	import Footer from '$lib/components/Footer/Footer.svelte'
	import Hero from '$lib/components/Hero/Hero.svelte'

	import SvgEmail from '$lib/svgs/email.svg?raw';
	import SvgPhone from '$lib/svgs/phone.svg?raw';

	import ImageVideo from '$lib/images/video.jpg'
</script>

<main class="p-home">
	<Hero />

	<!-- WHAT -->
	<section class="section-what">
		<div>
			<h2>
				<span>Guelph Process Serving specializes in Process Serving and Court Filing</span>
			</h2>
			<p>
				We service the City of Guelph and surrounding areas for the following courts:
			</p>
			<ul>
				<li>Small Claims Court</li>
				<li>Ontario Court of Justice</li>
				<li>Superior Court of Justicee</li>
				<li>Court Filing</li>
			</ul>
		</div>
		<div class="sub-section">
			<h2>
				<span>To get started</span>
			</h2>
			<p>
				Simply provide your document(s) and a memo outlining your instructions for process serving or court filing to Guelph Process Serving.
				Use any of the following ways to connect with us::
			</p>
			<div class="contacts">
				<div class="contact sub-section">
					<div class="contact-title">
						<div class="contact-svg">
							{@html SvgEmail}
						</div>
						<div class="contact-label">
							Email
						</div>
					</div>
					<div class="value">
						<a href="mailto:guelphprocessserving@rogers.com" rel="noreferrer" target="_blank">
							Our Email Address
						</a>
					</div>
				</div>
				<div class="contact sub-section">
					<div class="contact-title">
						<div class="contact-svg">
							{@html SvgEmail}
						</div>
						<div class="contact-label">
							Post
						</div>
					</div>
					<div>
						13 Robertson Dr., Guelph, ON, N1H 4S8
					</div>
				</div>
				<div class="contact sub-section">
					<div class="contact-title">
						<div class="contact-svg">
							{@html SvgPhone}
						</div>
						<div class="contact-label">
							Courier Pickup
						</div>
					</div>
					<div>
						<a href="tel:519-400-1479" rel="noreferrer" target="_blank" aria-label="Call 519-400-1479">
							519-400-1479
						</a>
					</div>
				</div>
			</div>
			<p>
				Once your documentation has been received we will promptly provide you with an Affidavit of Service or email confirmation of court filing.
			</p>
		</div>
	</section>


	<!-- FEES -->
	<section class="section-fees section-secondary sub-section">
		<h2>
			Fees
		</h2>
		<div>
			<div class="fees-section">
				<h3>Process Serving</h3>
				<div class="fees">
					<div class="fee">
						<div>Service including Commissioned Affidavit of Service within the City of Guelph</div>
						<div class="fee-value">$80</div>
					</div>
					<div class="fee">
						<div>Service including Commissioned Affidavit of Service outside the City of Guelph (up to 6 hour drive)</div>
						<div class="fee-value">$80 + $0.90/km</div>
					</div>
					<div class="fee">
						<div>Missed attempts at Service</div>
						<div class="fee-value">$30 per attempt</div>
					</div>
					<div class="fee">
						<div>Rush/same day Service</div>
						<div class="fee-value">add $35</div>
					</div>
				</div>
			</div>
			<div class="fees-section sub-section">
				<h3>Court Filing</h3>
				<div class="fees">
					<div class="fee">
						<div>Court Filing within the City of Guelph</div>
						<div class="fee-value">$30</div>
					</div>
					<div class="fee">
						<div>Filing outside the City of Guelph (up to 6 hour drive)</div>
						<div class="fee-value">$30 + $0.90/km</div>
					</div>
					<div class="fee">
						<div>Rush/same day Filing</div>
						<div class="fee-value">add $35</div>
					</div>
				</div>
			</div>
			<div class="fees-section  sub-section">
				<h3>Delivery</h3>
				<div class="fees">
					<div class="fee">
						<div>Delivery within the City of Guelph</div>
						<div class="fee-value">$20</div>
					</div>
					<div class="fee">
						<div>Mailing fee per 8x12 envelope</div>
						<div class="fee-value">$5</div>
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- ABOUT -->
	<section class="section-about">
		<h2>
			<span>About</span>
		</h2>
		<div>
			<div>
				<p>
					With over a decade of experience working in the legal field, we have the experience required to effectively, and efficiently handle your process serving and filing requirements. We have the relevant Knowledge of Family Law, Civil Litigation, and Small Claims to assist you in getting the job done right.
				</p>
				<p>
					Check out this video showing Guelph Process Serving in action:
				</p>
				<a href="http://vimeo.com/32691479" target="_blank" rel="noreferrer">
					<img class="video" src={ImageVideo} alt="The story behind Guelph Process Serving" />
				</a>
			</div>
		</div>
	</section>

	<Footer />
</main>

<style lang="css">
	.contact-title {
    	align-items: center;
		display: flex;
    	gap: var(--spacing-8);
	}

	.contact-svg {
		align-items: center;
		display: flex;
		fill: var(--color-black);
		justify-content: center;
		width: var(--spacing-32);
	}

	.fees-section {
		background-color: var(--color-white);
		border-radius:  var(--spacing-8);
		padding: var(--spacing-20);
	}

	.fees-section h3 {
		margin-bottom: var(--spacing-8);
	}

	.fees {
    	display: flex;
    	flex-direction: column;
    	gap: var(--spacing-8);
	}

	.fee-value {
		font-weight: var(--font-weight-bold);
	}

	.video {
		max-width: 600px;
		width: 100%;
	}
</style>