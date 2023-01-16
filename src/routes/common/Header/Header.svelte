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
    header{
        position: relative;
        display: flex;
        align-items: center;
        column-gap: 20px;
        height: 160px;
        width: 1130px;
        padding: 0 30px;
        margin: 0 auto;
        border-bottom: 1px solid #e4e8eb;
    }
</style>