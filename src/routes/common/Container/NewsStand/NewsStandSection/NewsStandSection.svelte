<div>
    <nav class="news-stand-title">
        <div class="presses">
            <img src="/images/NewsStand/newsIcon.png" alt="news-stand" />
            뉴스스탠드
            <img src="/images/arrow.png" alt="arrow" />
            <div>구독한 언론사</div>
            <div>전체언론사</div>
        </div>
        <div class="view-radios">
            <label>
                <input name="frame" type="radio" checked />
                <img src="/images/NewsStand/listIcon.png" alt="list-icon" />
            </label>
            <label>
                <input name="frame" type="radio" />
                <img src="/images/NewsStand/tileIcon.png" alt="tile-icon" />
            </label>
            <a href="/">
                <img src="/images/NewsStand/settingsIcon.png" alt="settings-icon" />
            </a>
        </div>
    </nav>
</div>

<style>
    nav {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 22px 0 16px;
    }
    .presses {
        display: flex;
        align-items: flex-end;
        column-gap: 5px;
    }
    .presses img:nth-child(1) {
        height: 20px;
    }
    .presses img:nth-child(2) {
        align-self: center;
        height: 10px;
    }
    .presses div:last-child {
        display: flex;
        align-items: center;
    }
    .presses div:last-child::before {
        content: '';
        display: inline-block;
        width: 4px;
        height: 4px;
        border-radius: 50%;
        margin-right: 8px;
        background-color: #c7ccd1;
    }

    .view-radios {
        display: flex;
        align-items: center;
        column-gap: 18px;
    }
    .view-radios label {
        display: flex;
        align-items: center;
    }
    .view-radios label input {
        display: none;
    }
    .view-radios label input:checked ~ img {
        filter: invert(38%) sepia(58%) saturate(870%) hue-rotate(192deg) brightness(85%) contrast(84%);
    }
    .view-radios img {
        width: 14px;
    }
</style>