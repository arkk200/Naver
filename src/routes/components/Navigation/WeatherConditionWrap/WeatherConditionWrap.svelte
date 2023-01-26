<script>
    import DustCondition from "./DustCondition.svelte";
    import WeatherCondition from "./WeatherCondition.svelte";

</script>

<div class="weather-condition-wrap">
    <div class="condition">
        <DustCondition />
        <WeatherCondition />
    </div>
</div>

<style lang="scss">
    .weather-condition-wrap {
        height: 52px;
        overflow: hidden;
        
        .condition {
            animation: slide 14s infinite;

            &:hover {
                animation-play-state: paused;
            }
        }
        @keyframes slide {
            from {
                transform: translateY(0);
            }
            47% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-50%);
            }
            97% {
                transform: translateY(-50%);
            }
        }
    }

</style>