<script>
	import { close, logo, menu } from '../assets';
	import { navLinks } from '../lib/index.js';
	import styles from '../lib/style.js';

	$: display = false;
</script>

<nav class="{styles.flexBetween} w-full navbar py-6">
	<img src={logo} alt="hoobank" class="w-[124px] h-[32px]" />
	<ul class="sm:flex hidden justify-end items-center flex-1 gap-10">
		{#each navLinks as nav}
			<li class="font-poppins font-normal text-white placeholder:text-lg">
				<a href={nav.id}>
					{nav.title}
				</a>
			</li>
		{/each}
	</ul>

	<div class="sm:hidden {styles.flexEnd} flex-1">
		<img
			on:click={() => (display = !display)}
			src={display ? close : menu}
			alt="menu"
			class="w-6 h-6 object-contain cursor-pointer"
		/>
		<div
			class={`${
				display ? 'flex' : 'hidden'
			} p-6 bg-black-gradient absolute top-20 right-0 mx-4 my-2 min-w-[140px] rounded-xl sidebar`}
		>
			<ul class="{styles.flexEnd} flex-col flex-1 gap-5">
				{#each navLinks as nav}
					<li class="font-poppins font-normal text-white placeholder:text-lg">
						<a href={nav.id}>
							{nav.title}
						</a>
					</li>
				{/each}
			</ul>
		</div>
	</div>
</nav>
