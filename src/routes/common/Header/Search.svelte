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

<style>
    .search-box {
        height: 56px;
        border: 2px solid #19ce60;
        display: flex;
    }
    .search-box .search-input {
        position: relative;
    }
    .search-box .search-input input {
        border: none;
        box-sizing: border-box;
        width: 444px;
        height: 100%;
        padding: 15px 13px;
    }
    .search-box .search-input span {
        position: absolute;
        top: 0;
        right: 40px;
        height: 100%;
        display: flex;
        align-items: center;
    }
    .search-box .search-input span:last-child {
        right: 8px;
    }
    .search-box .search-input span img {
        height: 24px;
    }
    .search-box input:focus {
        outline: none;
    }
    .search-box button {
        width: 56px;
        height: 56px;
        background-color: #19ce60;
        border: none;
    }
    .search-box button img {
        width: 22px;
    }
</style>