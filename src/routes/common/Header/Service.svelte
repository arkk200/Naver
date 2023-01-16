<div class="service">
    <a href="/">
        Logo를 시작페이지로
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

<style>
    .service {
        position: absolute;
        top: 12px;
        right: 27px;
        display: flex;
        align-items: center;
        width: 214px;
    }
    .service i {
        width: 1px;
        height: 10px;
        background-color: #e4e8eb;
        margin: 3px 7px;
    }
    .service a {
        font-family: 'Malgun Gothic';
        font-size: 11px;
        text-decoration: none;
        color: #404040;
    }
    .service > a {
        display: flex;
        align-items: center;
        column-gap: 6px;
    }
    .service > a span {
        width: 18px;
        height: 18px;
        border-radius: 50%;
        box-shadow: 0 1px 2px gray;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .service > a span img {
        height: 10px;
    }
    .service .add-ons {
        display: flex;
        column-gap: 6px;
    }
    .service .add-ons a {
        color: rgb(162, 162, 162);
    }
    .service .add-ons a:first-child:hover span:nth-child(1) {
        color: rgb(0, 81, 255);
    }
    .service .add-ons a:first-child:hover span:nth-child(2) {
        color: red;
    }
    .service .add-ons a:first-child:hover span:nth-child(3) {
        color: orange;
    }
    .service .add-ons a:first-child:hover span:nth-child(4) {
        color: #19ce60;
    }
    .service .add-ons a:last-child:hover {
        color: #15a74f;
    }
</style>