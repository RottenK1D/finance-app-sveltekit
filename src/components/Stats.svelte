<script>
	import { stats } from '../lib/index.js';
	import styles from '../lib/style.js';
</script>

<section class="{styles.flexCenter} flex-wrap sm:mb-20 mb-6 font-poppins">
	{#each stats as stat}
		<div class="flex justify-center items-center flex-1 m-3">
			<div
				class="font-semibold xs:text-[40px] text-[30px] xs:leading-[53px] leading-[43px] text-white"
			>
				{stat.value}
			</div>
			<div
				class="font-normal xs:text-[20px] text-[15px] xs:leading-[26px] leading-[21px] text-gradient uppercase ml-3"
			>
				{stat.title}
			</div>
		</div>
	{/each}
</section>
