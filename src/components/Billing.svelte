<script>
	import { apple, bill, google } from '../assets';
	import styles, { layout } from '../lib/style';
</script>

<section id="product" class={layout.sectionReverse}>
	<div class={layout.sectionImgReverse}>
		<img src={bill} alt="billing" class="w-full h-full relative z-[5]" />
		<div class="absolute z-[3] -left-1/2 top-0 w-[50%] h-[50%] rounded-full white__gradient" />
		<div class="absolute z-[0] -left-1/2 bottom-0 w-[50%] h-[50%] rounded-full pink__gradient" />
	</div>

	<div class="{layout.sectionInfo} ">
		<div class={styles.heading2}>
			Easily control your<br class="sm:block hidden" />
			billing & invoicing.
		</div>
		<div class="{styles.paragraph} max-w-[470px] mt-5">
			Elit enim sed massa etiam. Mauris eu adipiscing ultrices ametodio aenean neque. Fusce ipsum
			orci rhoncus aliporttitor integer platea placerat.
		</div>
		<div class="flex flex-wrap sm:mt-10 mt-6 gap-5">
			<img src={apple} alt="apple_store" class="w=[122px] h-[42px] object-contain cursor-pointer" />
			<img
				src={google}
				alt="google_store"
				class="w=[122px] h-[42px] object-contain cursor-pointer"
			/>
		</div>
	</div>
</section>
