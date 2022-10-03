<script>
	import styles, { layout } from '../lib/style.js';
	import FeedbackCard from './FeedbackCard.svelte';
</script>

<section id="clients" class="{styles.paddingY} {styles.flexCenter} flex-col relative">
	<div class="absolute z-0 w-[120%] h-[40%] rounded-full blue__gradient" />
	<div class="w-full {styles.flexCenter} md:flex-row flex-col sm:mb-16 mb-6 relative z-[1]">
		<div class={styles.heading2}>
			What people are<br class="sm:block hidden" />
			saying about us
		</div>
		<div class="w-full md:mt-0 mt-6">
			<div class="{styles.paragraph} text-left max-w-[450px]">
				Everything you need to accept card payments and grow your business anywhere on the planet.
			</div>
		</div>
	</div>
	<div class="flex flex-wrap sm:justify-start justify-center w-full relative z-[1]">
		<FeedbackCard />
	</div>
</section>
