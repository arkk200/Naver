<script>
    import PressesSelect from "./PressesSelect.svelte";
    import ViewRadios from "./ViewRadios.svelte";

</script>

<div class="news-stand-title">
    <PressesSelect />
    <ViewRadios />
</div>

<style>
    .news-stand-title {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 22px 0 16px;
        font-size: 14px;
    }
</style>