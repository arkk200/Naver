<script lang="ts">
    import Category from "./Category.svelte";
    
    let curCategoryNumber: number = 1;
    let pageByCategories = [81, 24, 12, 6, 24, 61, 35]
    const titleByCategories = ["종합/경재", "방송/통신", "IT", "영자지", "스포츠/연예계", "매거진/전문지", "지역"];
    const idByCategories = ["comprehensive/economic", "broadcast/communication", "IT", "english", "sports/entertainment", "magazine/tech-journal", "local"]
    export let page: number;

</script>

<div class="categories">
    {#each pageByCategories as pageNumber, i}
        <Category id={idByCategories[i]} bind:curCategoryNumber bind:page {pageNumber} bind:pageByCategories order={i+1}>{titleByCategories[i]}</Category>
    {/each}
    <!-- <Category id="broadcast/communication" bind:curCategoryNumber bind:page pageNumber={24} order={2}>방송/통신</Category>
    <Category id="IT" bind:curCategoryNumber bind:page pageNumber={12} order={3}>IT</Category>
    <Category id="english" bind:curCategoryNumber bind:page pageNumber={6} order={4}>영자지</Category>
    <Category id="sports/entertainment" bind:curCategoryNumber bind:page pageNumber={24} order={5}>스포츠/연예계</Category>
    <Category id="magazine/tech-journal" bind:curCategoryNumber bind:page pageNumber={61} order={6}>매거진/전문지</Category>
    <Category id="local" bind:curCategoryNumber bind:page pageNumber={35} order={7}>지역</Category> -->
</div>

<style>
    .categories {
        width: 163px;
        background: #f7f9fa;
        border: 1px solid #dae1e6;
        padding: 15px 0 0;
        display: flex;
        flex-direction: column;
        align-items: center;
        row-gap: 16px;
    }
</style>