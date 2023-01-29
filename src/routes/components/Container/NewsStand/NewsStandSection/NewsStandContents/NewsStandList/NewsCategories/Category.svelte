<script lang="ts">
    export let id: string, pageNumber: number, curCategoryNumber: number, page: number, pageByCategories: number[], order: number;

    $: if (curCategoryNumber === order && page > pageNumber) {
        curCategoryNumber += 1;
        curCategoryNumber %= 7;
        page = 1
    } else if (page < 1) {
        curCategoryNumber -= 1;
        curCategoryNumber < 1 && (curCategoryNumber = 7);
        page = pageByCategories[curCategoryNumber-1];
    }
</script>

<input {id} type="radio" name="category" checked={curCategoryNumber === order} on:change={() => {
    page = 1; curCategoryNumber = order
}} />
<label class="category" for={id}>
    <div class="category-name"><slot></slot></div>
    <div class="pages"><span>{page}</span> <span>/ {pageNumber}</span></div>
</label>

<style lang="scss">
    input[type=radio] {
        display: none;

        &:checked + .category {
            height: 34px;
            border-radius: 99px;
            background: #4063bd;
            font-weight: 700;
            color: white;

            .pages {
                display: block;
            }
        }
    }
    .category {
        cursor: pointer;
        width: 135px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 14px 0 18px;
        box-sizing: border-box;
        font-size: 13px;

        &:hover {
            .category-name {
                text-decoration: underline;
            }
        }
        
        .pages {
            display: none;
            font-size: 11px;

            span:last-child {
                opacity: .5;
            }
        }
    }
</style>