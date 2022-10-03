<script>
	import styles, { layout } from '../lib/style.js';
	import { card } from '../assets';
	import Button from './Button.svelte';
</script>

<section class={layout.section}>
	<div class={layout.sectionInfo}>
		<div class={styles.heading2}>
			Find a better card deal<br class="sm:block hidden" />
			in few easy steps.
		</div>
		<div class="{styles.paragraph} max-w-[470px] mt-5">
			Arcu tortor, purus in mattis at sed integer faucibus. Aliquet quis aliquet eget mauris
			tortor.ç Aliquet ultrices ac, ametau.
		</div>
		<div class="mt-5">
			<Button />
		</div>
	</div>
	<div class={layout.sectionImg}>
		<img src={card} alt="card" class="w-full h-full relative z-[5]" />
		<div class="absolute z-[3]  top-0 w-[50%] h-[50%] rounded-full white__gradient" />
		<div class="absolute z-[0]  bottom-0 w-[70%] h-[70%] rounded-full pink__gradient" />
	</div>
</section>
