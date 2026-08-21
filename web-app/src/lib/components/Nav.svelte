<script>
	import { base } from '$app/paths';
</script>

<div class="pt-6">
	<a href="{base}/" class="block pb-4">
		<!-- svelte-ignore a11y-img-redundant-alt -->
		<img
			src="{base}/logo.png"
			alt="Stylized version of The Double Scoop"
			width="300"
			height="30"
			class="mx-auto inset-0 flex items-center justify-center top-4"
		/>
	</a>
	<hr class="border-top border-black mb-1 pt" />
	<div class="text-center border border-black mb-5 shadow-[0_3px_3px_rgba(0,0,0,0.3)]">
		<div class="px-4 py-2 font-display font-semibold text-black text-base">
			<nav class="container mx-auto flex justify-evenly items-center">
				<a class="nav-link px-4 hover:text-red-500" href="{base}/">
					<img src="{base}/logo1.png" alt="Home" class="w-6 h-6 mr-1 inline" />
					<span>HOME</span>
				</a>
				<a class="nav-link px-4 hover:text-red-500" href="{base}/learn">
					<img src="{base}/logo2.png" alt="Learn" class="w-4 h-6 mr-1 inline" />
					<span>LEARN</span>
				</a>
				<a class="nav-link px-4 hover:text-red-500" href="{base}/stats">
					<img src="{base}/logo3.png" alt="Stats" class="w-6 h-6 mr-1 inline" />
					<span>STATS</span>
				</a>
				<a class="nav-link px-4 hover:text-red-500" href="{base}/contact">
					<img src="{base}/logo4.png" alt="Contact" class="w-6 h-6 mr-1 inline" />
					<span>CONTACT</span>
				</a>
			</nav>
		</div>
	</div>
</div>