<script lang="ts">
    import NewsStandTilePage from "./NewsStandTilePage.svelte";

    let page:number = 1
</script>

<div class="tile">
    
    {#if page > 1}
    <button class="prev" on:click={() => page--}>
        <img src="/images/arrow.png" alt="prev" />
    </button>
    {/if}
    {#if page < 4}
    <button class="next" on:click={() => page++}>
        <img src="/images/arrow.png" alt="prev" />
    </button>
    {/if}

    {#if page === 1}
        <NewsStandTilePage src="/images/NewsStand/nbclogo.png" alt="nbclogo" />
    {:else if page === 2}
        <NewsStandTilePage src="/images/NewsStand/nbslogo.png" alt="nbslogo" />
    {:else if page === 3}
        <NewsStandTilePage src="/images/NewsStand/nnnlogo.png" alt="nnnlogo" />
    {:else if page === 4}
        <NewsStandTilePage src="/images/NewsStand/nmologo.png" alt="nmologo" />
    {/if}
</div>

<style lang="scss">
    .tile {
        position: relative;
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