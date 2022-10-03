<script>
	import styles from '../lib/style';
	import Button from './Button.svelte';
</script>

<section
	class="{styles.flexCenter} {styles.marginY} {styles.padding} sm:flex-row flex-col bg-black-gradient-2 rounded-md box-shadow"
>
	<div class="flex flex-col flex-1">
		<div class={styles.heading2}>Let’s try our service now!</div>
		<div class="{styles.paragraph} max-w-[470px] mt-5">
			Everything you need to accept card payments and grow your business anywhere on the planet.
		</div>
	</div>
	<div>
		<Button />
	</div>
</section>
