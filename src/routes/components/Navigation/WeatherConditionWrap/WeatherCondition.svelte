<div class="weather-condition">
    <img src="/images/Navigation/weather.png" alt="weather-img" />
    <span class="temp">-1.4°</span>
    <span class="weather-status">맑음</span>
    <span class="min-temp">-8.0°</span>
    <span class="temp-sep">/</span>
    <span class="max-temp">-1.0°</span>
    을지로2가
</div>

<style>
    .weather-condition {
        position: relative;
        display: flex;
        align-items: center;
        justify-content: flex-end;
        column-gap: 5px;
        height: 52px;
        font-size: 12px;
        color: #808080;
    }
    .weather-condition span {
        font-size: 13px;
    }
    .weather-condition span.temp {
        font-size: 15px;
        font-weight: 900;
        color: #202020;
    }
    .weather-condition .weather-status {
        font-weight: 600;
        color: #202020;
    }
    .weather-condition .min-temp {
        color: rgb(0, 136, 255);
    }
    .weather-condition .temp-sep {
        color: #c1c5c9;
    }
    .weather-condition .max-temp {
        color: rgb(255, 17, 0);
    }
    .weather-condition img {
        height: 29px;
    }
</style>