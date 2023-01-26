<div class="service">
    <a href="/">
        Laver를 시작페이지로
        <span>
            <img src="/images/arrow.png" alt="arrow" />
        </span>
    </a>
    <i></i>
    <div class="add-ons">
        <a href="/">
            <span>쥬</span><span>니</span><span>어</span><span>로고</span>
        </a>
        <a href="/">해피빈</a>
    </div>
</div>

<style lang="scss">
    .service {
        position: absolute;
        top: 12px;
        right: 27px;
        display: flex;
        align-items: center;
        i {
            width: 1px;
            height: 10px;
            background-color: #e4e8eb;
            margin: 3px 7px;
        }
        a {
            font-family: 'Malgun Gothic';
            font-size: 11px;
            text-decoration: none;
            color: #404040;
        }
        > a {
            display: flex;
            align-items: center;
            column-gap: 6px;

            span {
                width: 18px;
                height: 18px;
                border-radius: 50%;
                box-shadow: 0 1px 2px gray;
                display: flex;
                align-items: center;
                justify-content: center;
                
                img {
                    height: 10px;
                }
            }
        }
        .add-ons {
            display: flex;
            column-gap: 6px;

            a {
                color: rgb(162, 162, 162);

                &:first-child:hover {
                    span {
                        &:nth-child(1) {
                            color: rgb(0, 81, 255);
                        }
                        &:nth-child(2) {
                            color: red;
                        }
                        &:nth-child(3) {
                            color: orange;
                        }
                        &:nth-child(4) {
                            color: #19ce60;
                        }
                    }
                }
                &:last-child:hover {
                    color: #15a74f;
                }
            }
        }
    }
</style>