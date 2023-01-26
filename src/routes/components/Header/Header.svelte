<script>
    import Logo from "./Logo.svelte";
    import Search from "./Search.svelte";
    import Service from "./Service.svelte";

</script>
<header>
    <div>
        <Logo />
        <Search />
        <Service />
    </div>
</header>

<style lang="scss">
    header {
        border-bottom: 1px solid #e4e8eb;
        
        div{
            position: relative;
            display: flex;
            align-items: center;
            column-gap: 20px;
            height: 160px;
            width: 1130px;
            padding: 0 30px;
            margin: 0 auto;
            box-sizing: border-box;
        }
    }
</style>