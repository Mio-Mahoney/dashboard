<script>
	import ScrollBox from './ScrollBox.svelte';

	const names = [
		'Ian Venton',
		'Eli Fereira',
		'Kerrie Little',
		'Mio Mahoney',
		'Ethan Browne',
		'Eli DeCampo',
		'Preston Precourt',
		'Jack Gallagher',
		'Olivia Perretto',
		'Joseph Vega',
		'Tiffany Cardoza',
		'Anthony Harter',
		'Luis Medina',
		'Victor Lockwood',
		'Landon Rusco',
		'Duncan Zaug',
		'Nex Dubose'
	];
</script>

<div class="text-[64px] text-[#E8B595] text-center">🦃 Happy Friendsgiving! 🦃</div>
<!-- Scrollable text -->
<div class="text-[#C39CAE] text-[32px] text-center">
	<p>
		Thank you for being a part of the CS Lounge! We are grateful for your presence. Happy
		Friendsgiving! <br />Thank you to:
	</p>
	<ScrollBox duration={50000}>
		<pre class=" whitespace-nowrap">
			{#each names as name}
				<span>{name} • </span>
			{/each}
		</pre>
	</ScrollBox>
</div>
