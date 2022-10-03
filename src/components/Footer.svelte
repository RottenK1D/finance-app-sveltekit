<script>
	import styles from '../lib/style';
	import { logo } from '../assets';
	import { footerLinks, socialMedia } from '../lib/index';
</script>

<section class="{styles.flexCenter} {styles.paddingY} flex-col">
	<div class="{styles.flexStart}  md:flex-row flex-col mb-8 w-full">
		<div class="flex flex-col flex-1 justify-start mr-10">
			<img src={logo} alt="logo" class="w-[266px] h-[72px] object-contain" />
			<div class="{styles.paragraph} mt-4 max-w-[310px]">
				A new way to make the payments easy, reliable and secure.
			</div>
		</div>

		<div class="flex-[1.5] w-full flex justify-between flex-wrap md:mt-0 mt-10 mb-10">
			{#each footerLinks as footer}
				<div class="flex flex-col ss:my-0 my-4 min-w-[150x] ">
					<div class="font-poppins font-medium text-[18px] leading-[28px] text-white mb-5">
						{footer.title}
					</div>
					<ul class="flex flex-col gap-2">
						{#each footer.links as link}
							<li
								class="font-poppins text-[16px] leading-[24px] text-dimWhite hover:text-secondary cursor-pointer"
							>
								{link.name}
							</li>
						{/each}
					</ul>
				</div>
			{/each}
		</div>
	</div>

	<div
		class="w-full {styles.flexBetween} md:flex-row flex-col pt-6 border-t-[1px] border-t-[#3F3E45]"
	>
		<div class="font-poppins text-[18px] leading-[28px] text-white text-center">
			2021 HooBank. All Rights Reserved.
		</div>
		<div class="flex md:mt-0 mt-6 gap-5">
			{#each socialMedia as media}
				<img
					key={media.id}
					src={media.icon}
					alt={media.id}
					class="w-[21px] h-[21px] object-contain cursor-pointer "
				/>
			{/each}
		</div>
	</div>
</section>
