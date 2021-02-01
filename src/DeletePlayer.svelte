<script>
	import { createEventDispatcher } from 'svelte';

    const dispatch = createEventDispatcher()
    const handleClick = (e) => {
        e.preventDefault()
        dispatch("deleteplayer")
    }
</script>

<button class="btn btn-sm" on:click={handleClick}>Delete Player</button>