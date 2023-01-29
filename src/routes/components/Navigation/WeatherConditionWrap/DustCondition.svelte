<div class="dust-condition">
    <span>미세</span>
    <div>
        <img src="/images/Navigation/findDustFace.png" alt="find-dust" />
        좋음
    </div>
    <i></i>
    <span>초미세</span>
    <div>
        <img src="/images/Navigation/findDustFace.png" alt="ultra-find-dust" />
        좋음
    </div>
    을지로 2가
</div>

<style lang="scss">
    .dust-condition {
        position: relative;
        display: flex;
        align-items: center;
        justify-content: flex-end;
        column-gap: 5px;
        height: 52px;
        font-size: 12px;
        color: var(--black04);
        span {
            color: var(--black03);
        }
        i {
            width: 1px;
            height: 12px;
            background-color: #E3E8EB;
        }
        div {
            display: flex;
            align-items: center;
            column-gap: 5px;
            font-size: 13px;
            font-weight: 900;
            color: var(--black01);
            img {
                height: 18px;
            }
        }
    }
</style>