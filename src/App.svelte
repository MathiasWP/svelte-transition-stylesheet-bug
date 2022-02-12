<script>
import {fade} from 'svelte/transition'

let visible = false;
</script>

<button on:click={() => visible = !visible}>Toggle visibility</button>

{#if visible}
    <div transition:fade>Hello!</div>
{/if}