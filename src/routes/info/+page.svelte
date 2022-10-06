<script>
	import { each } from 'svelte/internal';
	import json from './info.json';

	let list = json;
</script>

<div>
	<h1>Info</h1>

	<ul style="list-style-type: '--';">
		{#each list as item}
			<li style="display: flex;">
				<h4>{item.Key}</h4>
				<span>{item.value}</span>
			</li>
		{/each}
	</ul>
</div>
