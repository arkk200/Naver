<script lang="ts">
    export let src: string, alt: string;
</script>

<div class="page">
    {#each new Array(24) as _}
        <div>
            <img {src} {alt} />
        </div>
    {/each}
</div>

<style lang="scss">
    .page {
        width: 750px;
        height: 260px;
        display: grid;
        grid-template-columns: repeat(6, 1fr);
        grid-template-rows: repeat(4, 1fr);
        border-collapse: collapse;

        div {
            width: 100%;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            border: 0.5px solid #e4e8eb;
            img {
                height: 20px;
                position: relative;
                user-select: none;
            }
        }
    }
</style>