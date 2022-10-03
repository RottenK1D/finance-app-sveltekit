<script>
	import { features } from '../lib/index.js';
	import styles, { layout } from '../lib/style.js';
	import Button from './Button.svelte';
</script>

<section id="features" class={layout.section}>
	<div class={layout.sectionInfo}>
		<div class={styles.heading2}>
			You do the business<br class="sm:block hidden" />
			we’ll handle the money.
		</div>
		<div class="{styles.paragraph} max-w-[470px] mt-5">
			With the right credit card, you can improve your financial life by building credit, earning
			rewards and saving money. But with hundreds of credit cards on the market.
		</div>
		<div class="mt-8">
			<Button />
		</div>
	</div>

	<div class="{layout.sectionImg} flex-col">
		{#each features as feature}
			<div class="flex p-6 rounded-2xl gap-2 feature-card">
				<div class="w-[64px] h-[64px] rounded-full {styles.flexCenter} bg-dimBlue">
					<img src={feature.icon} alt="icon" class="w-[50%] h-[50%] object-contain" />
				</div>
				<div class="flex flex-1 flex-col ml-3 font-poppins">
					<div class="font-semibold text-white text-[18px] leading-[23px] mb-1">
						{feature.title}
					</div>
					<div class="text-dimWhite text-[16px] leading-[24px] ">
						{feature.content}
					</div>
				</div>
			</div>
		{/each}
	</div>
</section>
