<script lang="ts">
    import NewsStandList from "./NewsStandList/NewsStandList.svelte";
    import NewsStandTile from "./NewsStandTile/NewsStandTile.svelte";

     export let form: 'tile' | 'list';
     $: console.log(form);
</script>

<section>
    {#if form === "list"}
        <NewsStandList />
    {:else if form === "tile"}
        <NewsStandTile />
    {/if}
</section>