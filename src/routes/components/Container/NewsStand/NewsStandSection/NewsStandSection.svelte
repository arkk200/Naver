<script lang="ts">
    import NewsStandContents from "./NewsStandContents/NewsStandContents.svelte";
    import NewsStandTitle from "./NewsStandTitle/NewsStandTitle.svelte";
    let form: "tile" | "list" = "list";
</script>

<NewsStandTitle bind:form />
<NewsStandContents {form} />