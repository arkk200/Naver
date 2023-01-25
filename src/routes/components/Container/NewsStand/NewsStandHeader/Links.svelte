<div class="links">
    <a href="/">뉴스홈</a>
    <div class="other-links">
        <a href="/">연애</a>
        <a href="/">스포츠</a>
        <a href="/">경제</a>
    </div>
</div>

<style>
    .links {
        display: flex;
        margin-left: auto;
        column-gap: 4px;
    }
    .links a {
        font-size: 13px;
        text-decoration: none;
        color: #202020;
        font-weight: 600;
    }
    .links > a:first-child {
        color: #3565C9;
        display: flex;
        align-items: center;
    }
    .links > a:first-child::after {
        display: inline-block;
        width: 3px;
        height: 3px;
        content: '';
        background-color: #c8ccd1;
        border-radius: 50%;
        margin-left: 8px;
    }
    .links .other-links {
        display: flex;
        column-gap: 11px;
    }
</style>