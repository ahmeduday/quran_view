<div>
    <h1>Info</h1>

    <ul>
        {#each list as item}
            <li>
                <h4>{item.Key}</h4><span>{item.value}</span>
            </li>
        {/each}
    </ul>
</div>

<script>
    import { each } from 'svelte/internal';
import json from './info.json';

    let list = json;
</script>