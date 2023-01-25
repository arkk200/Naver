<script lang="ts">
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
    <div class="page page1">
        {#each new Array(24) as _}
            <div>
                <img src="/images/NewsStand/nbclogo.png" alt="nbclogo" />
            </div>
        {/each}
    </div>
    {:else if page === 2}
    <div class="page page2">
        {#each new Array(24) as _}
            <div>
                <img src="/images/NewsStand/nbslogo.png" alt="nbclogo" />
            </div>
        {/each}
    </div>
    {:else if page === 3}
    <div class="page page3">
        {#each new Array(24) as _}
            <div>
                <img src="/images/NewsStand/nnnlogo.png" alt="nbclogo" />
            </div>
        {/each}
    </div>
    {:else if page === 4}
    <div class="page page4">
        {#each new Array(24) as _}
            <div>
                <img src="/images/NewsStand/nmologo.png" alt="nbclogo" />
            </div>
        {/each}
    </div>
    {/if}
</div>

<style>
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
    .prev img, .next img {
        height: 20px;
    }
    .prev {
        left: -27px;
        transform: rotateZ(180deg) translateY(50%);
        box-shadow: 0 -2px 3px 1px #ddd;
    }
    .next {
        right: -13px;
        transform: translateY(-50%);
        box-shadow: 0 2px 3px 1px #ddd;
    }

    .page {
        width: 750px;
        height: 260px;
        display: grid;
        grid-template-columns: repeat(6, 1fr);
        grid-template-rows: repeat(4, 1fr);
        border-collapse: collapse;
    }
    
    .page div {
        width: 100%;
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        border: 0.5px solid #e4e8eb;
    }

    .page img {
        height: 20px;
        position: relative;
        user-select: none;
    }
</style>