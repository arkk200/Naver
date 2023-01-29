<script lang="ts">
    import CategoryContents from "./CategoryContents/CategoryContents.svelte";
    import NewsCategories from "./NewsCategories/NewsCategories.svelte";

    let page:number = 1;
</script>

<div class="list">
    <button class="prev" on:click={() => page--}>
        <img src="/images/arrow.png" alt="prev" />
    </button>
    <button class="next" on:click={() => page++}>
        <img src="/images/arrow.png" alt="prev" />
    </button>

    <NewsCategories bind:page />
    <CategoryContents />
</div>

<style lang="scss">
    .list {
        position: relative;
        height: 260px;
        display: flex;
    }
    .prev, .next {
        position: absolute;
        width: 44px;
        height: 44px;
        border: none;
        padding: 0;
        top: 50%;
        background-color: #fff;
        border-radius: 50%;
        cursor: pointer;
    }
    .prev {
        left: -27px;
        transform: rotateZ(180deg) translateY(50%);
        box-shadow: 0 -2px 3px 1px #ddd;
        
        img {
            height: 20px;
        }
    }
    .next {
        right: -13px;
        transform: translateY(-50%);
        box-shadow: 0 2px 3px 1px #ddd;

        img {
            height: 20px;
        }
    }
</style>