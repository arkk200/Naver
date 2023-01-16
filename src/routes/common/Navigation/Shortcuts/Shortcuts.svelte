<script>
    import AddOns from "./AddOns.svelte";
    import Favorites from "./Favorites.svelte";
    import ShowMore from "./ShowMore.svelte";

</script>
<div class="shortcuts">
    <AddOns />
    <Favorites />
    <ShowMore />
</div>

<style>
    .shortcuts {
        display: flex;
        align-items: center;
        column-gap: 12px;
    }
</style>