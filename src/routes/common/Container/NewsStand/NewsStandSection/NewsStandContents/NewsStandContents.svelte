<script lang="ts">
    import NewsStandList from "./NewsStandList/NewsStandList.svelte";
    import NewsStandTile from "./NewsStandTile/NewsStandTile.svelte";

     export let form: 'tile' | 'list';
     $: console.log(form);
</script>

<section>
    {#if form === "tile"}
        <NewsStandTile />
    {:else if form === "list"}
        <NewsStandList />
    {/if}
</section>