<script>
	import { base } from '$app/paths';
	import Nav from '$lib/components/Nav.svelte';
	import PageContainer from '$lib/components/PageContainer.svelte';

	let members = [
		{
			name: 'Indira Mariya',
			role: 'Developer',
			blurb: 'I like coding. My favorite flavor of ice cream is vanilla.',
			image: `${base}/CACindira.png`,
			border: 'rgb(190, 137, 250)',
			background: 'rgba(190, 137, 250, 0.2)'
		},
		{
			name: 'Sabrina Yen-Ko',
			role: 'Developer',
			blurb:
				'Vestibulum cursus ultricies nulla, ut vehicula ligula iaculis at. Fusce tristique malesuada.',
			image: `${base}/CACsabrina.png`,
			border: '#4fb880',
			background: 'rgba(79, 184, 128, 0.1)'
		},
		{
			name: 'Leo Troin',
			role: 'Designer',
			blurb:
				'Aenean a libero elit. Phasellus egestas vel elit id bibendum. Vivamus bibendum euismod dui.',
			image: `${base}/CACleo.png`,
			border: 'rgb(244, 175, 98)',
			background: 'rgba(244, 175, 98, 0.3)'
		},
		{
			name: 'Kaitlyn Don',
			role: 'Designer',
			blurb:
				'Aenean a libero elit. Phasellus egestas vel elit id bibendum. Vivamus bibendum euismod dui.',
			image: `${base}/CACkaitlyn.png`,
			border: 'rgb(255, 174, 207)',
			background: 'rgba(255, 174, 207, 0.2)'
		}
	];
</script>

<PageContainer>
	<header>
		<Nav />
	</header>
	<h1 class="pb-5 text-4xl">Meet the Team</h1>

	<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4">
		{#each members as member (member.name)}
			<div
				class="bg-white shadow-md p-4 rounded-lg"
				style="border: {member.border} solid 2px; background-color: {member.background};"
			>
				<img src={member.image} alt={member.name} class="w-full h-auto" />
				<h2 class="text-xl font-semibold mt-2">{member.name}</h2>
				<p class="text-gray-600">{member.role}</p>
			</div>
		{/each}
	</div>
</PageContainer>