<script lang="ts">
    export let form: "tile" | "list";
    function onChange(e: Event) {
        form = ((e.target as HTMLInputElement).value) as "tile" | "list";
    }
</script>

<div class="view-radios">
    <label>
        <input on:change={onChange} name="frame" value="list" type="radio" checked />
        <img src="/images/NewsStand/listIcon.png" alt="list-icon" />
    </label>
    <label>
        <input on:change={onChange} name="frame" value="tile" type="radio" />
        <img src="/images/NewsStand/tileIcon.png" alt="tile-icon" />
    </label>
    <a href="/">
        <img src="/images/NewsStand/settingsIcon.png" alt="settings-icon" />
    </a>
</div>

<style lang="scss">
    .view-radios {
        display: flex;
        align-items: center;
        column-gap: 18px;
        label {
            display: flex;
            align-items: center;
            input {
                display: none;
                &:checked ~ img {
                    filter: invert(38%) sepia(58%) saturate(870%) hue-rotate(192deg) brightness(85%) contrast(84%);
                }
            }
        }
        img {
            width: 14px;
        }
    }
</style>