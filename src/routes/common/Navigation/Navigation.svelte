<script>
    import Condition from "./Condition/Condition.svelte";
import Shortcuts from "./Shortcuts/Shortcuts.svelte";

</script>
<nav>
    <Shortcuts />
    <div class="condition-wrap">
        <Condition />
    </div>
</nav>

<style>
    nav{
        width: 1130px;
        height: 52px;
        padding: 0 30px;
        margin: 0 auto;
        display: flex;
        align-items: center;
        justify-content: space-between;
        font-size: 15px;
        box-shadow: 0 1px 3px 0 rgb(0 0 0 / 12%);
    }
    .condition-wrap {
        height: 52px;
        overflow: hidden;
    }
</style>