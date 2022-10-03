<script>
	import styles from '../lib/style.js';
	import {
		Hero,
		Stats,
		Business,
		Billing,
		CardDeal,
		Testimonials,
		Clients,
		CTA,
		Footer,
		Navbar
	} from '../components';
</script>

<div class="bg-primary w-screen overflow-hidden">
	<div class="{styles.paddingX} {styles.flexCenter}">
		<div class={styles.boxWidth}>
			<Navbar />
		</div>
	</div>
	<div class={styles.flexStart}>
		<div class={styles.boxWidth}><Hero /></div>
	</div>

	<div class="{styles.flexStart} {styles.paddingX}">
		<div class={styles.boxWidth}>
			<Stats />
			<Business />
			<Billing />
			<CardDeal />
			<Testimonials />
			<Clients />
			<CTA />
			<Footer />
		</div>
	</div>
</div>
