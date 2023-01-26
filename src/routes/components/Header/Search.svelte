<div class="search-box">
    <div class="search-input">
        <input />
        <span>
            <img src="/images/keyboardbright.png" alt="keyboard" />
        </span>
        <span>
            <img src="/images/autocompleteArrow.png" alt="keyboard" />
        </span>
    </div>
    <button>
        <img src="/images/search.png" alt="search" />
    </button>
</div>

<style lang="scss">
    .search-box {
        height: 56px;
        width: 586px;
        border: 2px solid #19ce60;
        display: flex;
        justify-content: space-between;

        .search-input {
            position: relative;
            flex: 1;

            input {
                border: none;
                box-sizing: border-box;
                width: 474px;
                height: 100%;
                padding: 15px 13px;
            }
            span {
                position: absolute;
                top: 0;
                right: 40px;
                height: 100%;
                display: flex;
                align-items: center;

                &:last-child {
                    right: 8px;
                }
                img {
                    height: 24px;
                }
            }
        }
        input:focus {
            outline: none;
        }
        button {
            width: 56px;
            height: 56px;
            background-color: #19ce60;
            border: none;
            img {
                width: 22px;
            }
        }
    }
</style>