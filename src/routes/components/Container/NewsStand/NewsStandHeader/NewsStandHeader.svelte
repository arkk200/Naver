<script>
    import Links from "./Links.svelte";
import NewsHeaderContents from "./NewsHeaderContents.svelte";
import NewsMedia from "./NewsMedia.svelte";
</script>

<header class="news-stand-header">
    <NewsMedia />
    <div class="news-header-contents-wrap">
        <NewsHeaderContents />
    </div>
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

    .news-header-contents-wrap {
        height: 24px;
        overflow: hidden;
    }
</style>