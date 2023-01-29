<script>
    import Container from './components/Container/Container.svelte';
    import Header from './components/Header/Header.svelte';
    import Navigation from './components/Navigation/Navigation.svelte';
</script>

<div class="wrap">
    <Header />
    <Navigation />
    <Container />
</div>

<style>
    .wrap {
        min-width: 1190px;
    }
    :global(:root) {
        --naver-color: #19ce60;
        --black01: #202020;
        --black02: #404040;
        --black03: #505050;
        --black04: #808080;
    }
</style>