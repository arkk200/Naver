<div class="links">
    <a href="/">뉴스홈</a>
    <div class="other-links">
        <a href="/">연애</a>
        <a href="/">스포츠</a>
        <a href="/">경제</a>
    </div>
</div>

<style lang="scss">
    .links {
        display: flex;
        margin-left: auto;
        column-gap: 4px;

        a {
            font-size: 13px;
            text-decoration: none;
            color: var(--black01);
            font-weight: 600;
        }
        > a:first-child {
            color: #3565C9;
            display: flex;
            align-items: center;

            &::after {
                display: inline-block;
                width: 3px;
                height: 3px;
                content: '';
                background-color: #c8ccd1;
                border-radius: 50%;
                margin-left: 8px;
            }
        }
        .other-links {
            display: flex;
            column-gap: 11px;
        }
    }
</style>