<script>
	import styles from '../lib/style';
	import { clients } from '../lib/index';
</script>

<section class="{styles.flexCenter} my-4">
	<div class="{styles.flexCenter} flex-wrap w-full">
		{#each clients as client}
			<div class="{styles.flexCenter} flex-1 min-w-[120px]">
				<img src={client.logo} alt="client" class="sm:w-[192px] w-[100px] object-contain" />
			</div>
		{/each}
	</div>
</section>
