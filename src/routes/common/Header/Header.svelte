<script>
    import Logo from "./Logo.svelte";
    import Search from "./Search.svelte";
    import Service from "./Service.svelte";

</script>
<header>
    <Logo />
    <Search />
    <Service />
</header>

<style>
    header {
        position: relative;
        display: flex;
        align-items: center;
        column-gap: 20px;
        height: 160px;
        width: 100vw;
        padding: 0 30px;
        box-sizing: border-box;
    }
</style>