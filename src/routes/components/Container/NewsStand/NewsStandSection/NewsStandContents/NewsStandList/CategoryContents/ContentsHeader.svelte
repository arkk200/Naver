<div class="contents__header">
    <div class="press-logo">
        <img src="/images/NewsStand/nbclogo.png" alt="logo" />
    </div>
    <div>2023.01.27. 03:10 편집</div>
    <button class="subscribe-btn">
        <span>+</span>
        <span>구독하기</span>
    </button>
</div>

<style lang="scss">
    .contents__header {
        grid-column: 1 / 3;
        display: flex;
        align-items: center;
        column-gap: 10px;
        font-size: 12px;
        color: #808080;

        .press-logo {
            img {
                height: 20px;
                cursor: pointer;
            }
        }

        .subscribe-btn {
            background: #F7F9FA;
            border: 1px solid #e4e8eb;
            height: 100%;
            border-radius: 99px;
            display: flex;
            align-items: center;
            column-gap: 2px;
            cursor: pointer;
            padding: 3px 12px 2px 11px;

            span {
                font-size: 11px;
                font-weight: 350;

                &:first-child {
                    font-size: 16px;
                    color: var(--naver-color);
                }
            }
        }
    }
</style>