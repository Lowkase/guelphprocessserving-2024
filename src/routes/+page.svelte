<script>
	import about from '$lib/svgs/about.svg?raw';
	import benefits from '$lib/svgs/benefits.svg?raw';
	import bodymind from '$lib/svgs/bodymind.svg?raw';
	import calendar from '$lib/svgs/calendar.svg?raw';
	import fees from '$lib/svgs/fees.svg?raw';
	import treatments from '$lib/svgs/treatments.svg?raw'; 

	import mike from '$lib/images/mike.jpeg'
	import myfm from '$lib/images/myfm-spirit-award.png'

	import Header from '$lib/components/Header.svelte'
	import Footer from '$lib/components/Footer.svelte'
	import Hero from '$lib/components/Hero.svelte'
	import ButtonLink from '$lib/components/ButtonLink.svelte'
</script>

<main class="p-home">
	<Header />
	<Hero />

	<!-- TREATMENTS / FEES -->
	<section class="section-treatment">
		<div class="m-col m-col-2">
			<div>
				<h2>
					{@html treatments}
					<span>Treatments</span>
				</h2>
				<p>
					After a careful assessment and consultation, we will create your treatment plan using one or 
					more of the following techniques:
				</p>
				<ul>
					<li>Swedish massage</li>
					<li>Remedial exercises</li>
					<li>Manual Lymphatic Drainage</li>
					<li>Friction and Trigger Point Therapy</li>
					<li>Sports Massage</li>
					<li>Fascial Work</li>
				</ul>
				<ButtonLink
					link="https://mikevecchiormt.clinicsense.com/book"
					scheme="m-button-content"
					svgShow={true}
					svgSvg={calendar}
					text="BOOK AN APPOINTMENT"
				/>
			</div>
			<div>
				<h2>
					{@html fees}
					<span>Fees</span>
				</h2>
				<ul>
					<li>30 minutes - $60</li>
					<li>45 minutes - $75</li>
					<li>60 minutes - $90</li>
					<li>75 minutes - $120</li>
				</ul>
			</div>
		</div>
	</section>


	<!-- BENEFITS -->
	<section class="section-benefits section-secondary">
		<h2>
			{@html benefits}
			<span>Benefits of Massage</span>
		</h2>
		<div class="benefits-list">
			<div class="benefit-list-item">
				<h3>Everyone</h3>
				<div>
					Massage therapy offers numerous benefits to the entire body. It helps ease joint and muscle pain, 
					and can help with natural pain control, blood pressure issues, boost your immune system, flush 
					toxins, and assist in injury healing.
				</div>
			</div>
			<div class="benefit-list-item">
				<h3>Athletes</h3>
				<div>
					Involved in sports? Specific treatments tailored to improving and maintaining a healthy body. Focussing on 
					stretching and strengthening is key to a healthy athlete. Maintenance treatments will keep you active and 
					happy!
				</div>
			</div>
			<div class="benefit-list-item">
				<h3>Seniors</h3>
				<div>
					The massage techniques utilized for seniors include lighter, gentle stroking and kneading as well as 
					application of pressure to specific points on the body. Even the most gentle massage has proven effects 
					on the nervous system and blood circulation, two of the most vulnerable systems of the body that feel 
					the effects of aging.  A typical massage for a senior usually involves a short session lasting around 
					thirty minutes.
				</div>
			</div>
		</div>
	</section>


	<!-- BODY AND MIND -->
	<section class="section-body-and-mind">
		<h2>
			{@html bodymind}
			<span>Body and Mind</span>
		</h2>
		<div class="m-col m-col-2">
			<div>
				<h3>Increase</h3>
				<ul>
					<li>Pain control</li>
					<li>Quality of sleep</li>
					<li>Immune system</li>
					<li>Respiratory function</li>
					<li>Circulation</li>
					<li>Joint range of motion (ROM)</li>
					<li>Flexibility</li>
					<li>Sense of well-being</li>
				</ul>
			</div>
			<div>
				<h3>Decrease</h3>
				<ul>
					<li>Stress and anxiety</li>
					<li>Blood pressure</li>
					<li>Muscle tension</li>
					<li>Neurological excitability (nerves more relaxed)</li>
					<li>Muscle spasms</li>
				</ul>
			</div>
		</div>
	</section>


	<!-- ABOUT -->
	<section class="section-secondary">
		<h2>
			{@html about}
			<span>About</span>
		</h2>
		<p>
			<img class="image-mike" src={mike} alt="Portrait of Mike Vecchio" /> My interest in massage therapy 
			began nearly 20 years ago after two motor vehicle accidents.  
			With massage therapy, physiotherapy and other modalities, I was able to return to a healthy me.  
			Since then massage has always been important to me, both physically and mentally.  As an RMT I 
			look forward to working with my clients in a relaxing, calm and welcoming environment. Our lives 
			today can be overwhelming, and massage gives us that chance to unwind, focus on what our bodies 
			are telling us, and allow us to heal and relax.
		</p>
		<p>
			As a husband, father of 5, and grandfather, I know how busy and stressful life can be. It’s 
			important to look after ourselves, so we can feel our best to take on what life offers with 
			enthusiasm!                        
		</p>
		<p>
		I graduated with honours from Westervelt College Massage Therapy Program in 2019. I enjoy 
		working with clients of all ages to assist in promoting a healthier life, providing relaxation 
		and treating various issues. In my spare time I enjoy being outdoors, gardening and fishing, 
		and hikes with my wife!
		</p>
		<p>
			&#34;The practice of Massage Therapy is the assessment of the soft tissue and joints of the body 
			and the treatment and prevention of physical dysfunction and pain of the soft tissue and joints 
			by manipulation to develop, maintain, rehabilitate or augment physical function, or relieve pain.&#34; 
			(Massage Therapy Act, 1991)
		</p>
		<p>
			&#34;Massage therapy consists primarily of hands-on manipulation of the soft tissues of the body, 
			specifically, the muscles, connective tissue, tendons, ligaments and joints for the purpose of 
			optimizing health. Massage therapy treatment has a therapeutic effect on the body and optimizes 
			health and well-being by acting on the muscular, nervous and circulatory systems. Physical function 
			can be developed, maintained and improved; and physical dysfunction and pain and the effects of 
			stress can be relieved or prevented through the use of Massage Therapy. Various specialized 
			movements of the hands, over the skin or clothes, make up the Massage Therapy treatment. The 
			Massage Therapist will work with your level of pain tolerance during the treatment, and the 
			treatment can be stopped at any time should the treatment become 
			uncomfortable.&#34; <a href="http://www.cmto.com" target="_blank" rel="noopener noreferrer">&#40;www.cmto.com&#41;</a>
		</p>
	</section>

	<!-- MYFM -->
	<section class="section-myfm">
		<img class="image-myfm" src={myfm} alt="Voted best Massage Therapist, Mike Vecchio" />
		<div class="text-myfm">Voted best Massage Therapist, Mike Vecchio</div>
	</section>

	<Footer />
</main>

<style>
	:global(.section-treatment .m-button) {
		margin-top: var(--spacing-36);
	}

	.benefit-list-item {
		margin-bottom: var(--spacing-28);
	}

	.image-mike {
		border-radius: var(--spacing-8);
		float: left;
		margin-bottom: var(--spacing-4);
		margin-right: var(--spacing-20);
		width: 180px;

		@media (max-width: 600px) {
			float: none;
			width: 100%;
		}
	}

	.section-myfm {
		display: flex;
		flex-direction: column;
		align-items: center;
		text-align: center;
	}

	.image-myfm {
		width: 320px;
		max-width: 100%;
	}
	@media (min-width: 768px) {
		.image-myfm {
			width: 300px;
		}
	}

	.text-myfm {
		color: var(--color-black);
		font-weight: var(--font-weight-medium);
	}
</style>