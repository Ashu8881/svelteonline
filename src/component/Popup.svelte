<script>

    import { createEventDispatcher } from "svelte";
    const dispatch = createEventDispatcher();
</script>
<div>
<h2>this is popup</h2>
<button on:click={() => dispatch ('close','Ashutosh')}>Close popup</button>
</div>