<script>
	import { feedback } from '../lib/index.js';
	import { quotes } from '../assets';
</script>

{#each feedback as card}
	<div
		class="flex justify-between flex-col px-10 py-12 rounded-md max-w-[370px] md:mr-10 sm:mr-5 mr-0 my-5 feedback-card"
	>
		<img src={quotes} alt="double_quotes" class="w-[42px] h-[28px] object-contain" />
		<div class="font-poppins font-normal text-[18px] leading-[32px] text-white my-10">
			{card.content}
		</div>
		<div class="flex">
			<img src={card.img} alt={card.name} class="w-[48px] h-[48px] rounded-full" />
			<div class="flex flex-col ml-4">
				<div class="font-poppins font-semibold text-[21px] leading-[32px] text-white">
					{card.name}
				</div>
				<div class="font-poppins font-normal text-[16px] leading-[24px] text-dimWhite">
					{card.title}
				</div>
 			</div>
		</div>
	</div>
{/each}
