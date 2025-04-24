<script lang="ts">

    interface Props {
        data: {
            entries: string[];
        }
    }

	const { data }: Props = $props();
    
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>
{#each data.entries as entry}
	<h1>{entry}</h1>
{/each}
