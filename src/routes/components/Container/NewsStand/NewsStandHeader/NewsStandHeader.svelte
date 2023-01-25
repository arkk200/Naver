<script>
    import Links from "./Links.svelte";
import NewsHeaderContents from "./NewsHeaderContents.svelte";
import NewsMedia from "./NewsMedia.svelte";
</script>

<header class="news-stand-header">
    <NewsMedia />
    <NewsHeaderContents />
    <Links />
</header>

<style>
    .news-stand-header {
        padding: 12px 15px 11px;
        background-color: #F7F9FA;
        border: 1px solid #DAE1E6;
        display: flex;
        align-items: center;
    }
</style>