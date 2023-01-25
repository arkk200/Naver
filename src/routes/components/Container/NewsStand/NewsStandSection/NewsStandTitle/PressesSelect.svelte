<div class="presses-select">
    <img src="/images/NewsStand/newsIcon.png" alt="news-stand" />
    <p>뉴스스탠드</p>
    <img src="/images/arrow.png" alt="arrow" />
    <label>
        <input name="presses-type" type="radio" checked />
        <p>구독한 언론사</p>
    </label>
    <label>
        <input name="presses-type" type="radio" />
        <p>전체언론사</p>
    </label>
</div>

<style>
    .presses-select {
        display: flex;
        align-items: flex-end;
        column-gap: 5px;
    }
    .presses-select > p {
        font-weight: 600;
    }
    .presses-select img:nth-child(1) {
        height: 20px;
    }
    .presses-select img:nth-child(3) {
        align-self: center;
        height: 10px;
    }
    .presses-select label:last-child {
        display: flex;
        align-items: center;
    }
    .presses-select label:last-child::before {
        content: '';
        display: inline-block;
        width: 4px;
        height: 4px;
        border-radius: 50%;
        margin-right: 8px;
        background-color: #c7ccd1;
    }
    .presses-select label input {
        display: none;
    }
    .presses-select label input:checked ~ p {
        font-weight: 600;
    }
</style>