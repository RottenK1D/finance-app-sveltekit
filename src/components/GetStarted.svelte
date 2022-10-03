<script>
	import styles from '../lib/style.js';
	import { arrowUp } from '../assets';
</script>

<div class="{styles.flexCenter} w-36 h-36 rounded-full bg-blue-gradient p-0.5 cursor-pointer">
	<div class="{styles.flexCenter} flex-col bg-primary w-full h-full rounded-full">
		<div class="{styles.flexStart} gap-3">
			<div class="font-poppins font-medium text-[18px] leading-[20px]">
				<span class="text-gradient">Get</span>
			</div>
			<img src={arrowUp} alt="arrow" class="w-6 h-6 object-contain" />
		</div>
		<div class="font-poppins font-medium text-[18px] leading-[20px]">
			<span class="text-gradient">Started</span>
		</div>
	</div>
</div>
