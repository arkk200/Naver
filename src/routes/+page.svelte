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
</style>