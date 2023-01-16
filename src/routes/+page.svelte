<script>
    import Container from './common/Container/Container.svelte';
    import Header from './common/Header/Header.svelte';
    import Navigation from './common/Navigation/Navigation.svelte';
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