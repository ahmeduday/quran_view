<script>
	import { each } from 'svelte/internal';
	import json from '../../data/chapters.json';
    import {Book, PlayFill, InfoCircleFill} from "svelte-bootstrap-icons";

</script>

<div>
	<h1>Chapters</h1>

	<ul style="list-style-type: none;">
		{#each json as item}
			<li >
                <div style="display: flex; margin:20px;">
                    <span>{item.key}. </span>
                    <span>{item.value}</span>
                    <span style="margin-right: 100px;"></span>
                    <Book style="margin-right:20px;"/>
                    <PlayFill color="red" style="margin-right:20px;"/>
                    <InfoCircleFill color="blue" style="margin-right:20px;"/>
                </div>
                <hr>
			</li>
		{/each}
	</ul>
</div>
