<script>
	import styles from '../lib/style.js';
	import { discount, robot } from '../assets';
	import { GetStarted } from '../components';
</script>

<section id="home" class="flex flex-col md:flex-row {styles.paddingY}">
	<div class="{styles.flexStart} flex-1 flex-col xl:px-0 sm:px-16 px-6">
		<div class="flex flex-row items-center py-1.5 px-4 bg-discount-gradient rounded-xl mb-10">
			<img src={discount} alt="discount" class="w-8 h-8" />
			<p class="{styles.paragraph} ml-2">
				<span class="text-white ">20%</span>&nbsp;DISCOUNT FOR&nbsp;
				<span class="text-white">1 Month</span>&nbsp; ACCOUNT
			</p>
		</div>

		<div class="{styles.flexBetween} w-full">
			<div
				class="flex-1 font-poppins font-bold ss:text-[72px] text-[52px] text-white ss:leading-[80px] leading-[50px]"
			>
				The Next <br class="sm:block hidden " />
				<span class="text-gradient">Generation</span><br />
				<span>Payment Method</span>
			</div>
			<div class="ss:flex self-start hidden md:mr-4 mr-0 ml-10">
				<GetStarted />
			</div>
		</div>
		<div class="{styles.paragraph} max-w-[470px] mt-5">
			With the right credit card, you can improve your financial life by building credit, earning
			rewards and saving money. But with hundreds of credit cards on the market.
		</div>
	</div>

	<div class="flex flex-1 {styles.flexCenter} md:my-0 my-10 relative">
		<img src={robot} alt="billing" class="w-full h-full relative z-[5]" />
		<div class="absolute z-[0] w-[40%] h-[35%] top-0 pink__gradient" />
		<div
			class="absolute z-[1] w-[80%] h-[80%] bottom-40 pink__gradient rounded-full white__gradient"
		/>
		<div class="absolute z-[0] w-[50%] h-[50%] right-20 bottom-20 blue__gradient" />
	</div>

	<div class="ss:hidden {styles.flexCenter}">
		<GetStarted />
	</div>
</section>
