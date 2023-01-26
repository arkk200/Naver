<script>
    import Category from "./Category.svelte";

</script>

<div class="categories">
    <Category id="comprehensive/economic" pagesNumber={81} checked>종합/경재</Category>
    <Category id="broadcast/communication" pagesNumber={24}>방송/통신</Category>
    <Category id="IT" pagesNumber={12}>IT</Category>
    <Category id="english" pagesNumber={6}>영자지</Category>
    <Category id="sports/entertainment" pagesNumber={24}>스포츠/연예계</Category>
    <Category id="magazine/tech-journal" pagesNumber={61}>매거진/전문지</Category>
    <Category id="local" pagesNumber={35}>지역</Category>
</div>

<style>
    .categories {
        width: 163px;
        background: #f7f9fa;
        border: 1px solid #dae1e6;
        padding: 21px 0 0;
        display: flex;
        flex-direction: column;
        align-items: center;
        row-gap: 16px;
    }
</style>