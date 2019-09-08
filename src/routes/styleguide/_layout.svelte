<script>
    import Content from '../../components/UI/Content.svelte';
    import Spacer from '../../components/UI/Spacer.svelte';

    import Navigation from '../../components/Styleguide/Navigation.svelte';

    // General
    let debug = false;

    // Styleguide related
    let styleguide = false;

    export let segment;

</script>

<style>

    .grid-layout {
        display: grid;
        grid-gap: 2rem;
        grid-template-columns: 30rem minmax(30rem, 1fr);
        height: 100%;
    }

    .grid-item {
        padding: 2rem;
    }

    .is-scrollable {
        height: 100%;
        overflow: scroll;
    }
</style>

<svelte:head>
	<title>Style guide</title>
</svelte:head>

<div class="grid-layout">
    <div class="grid-item is-scrollable">
        <Spacer side="top">
            <h1 class="c-h4">Table of Contents</h1>
            <Navigation segment="{segment}" />
        </Spacer>
    </div>
    <div class="grid-item is-scrollable">
        <div id="components">
            <slot></slot>
        </div>
    </div>
</div>
