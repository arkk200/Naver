<script>
    import ContentsHeader from "./ContentsHeader.svelte";

</script>
<div class="category-contents">
    <ContentsHeader />
</div>

<style lang="scss">
    .category-contents {
        flex: 1;
        border-top: 1px solid #dae1e6;
        border-bottom: 1px solid #dae1e6;
        padding: 17px 24px;
        display: grid;
        grid-template-columns: 196px 317px;
        column-gap: 24px;
        grid-template-rows: 27px 193px;
        row-gap: 6px;
    }
</style>