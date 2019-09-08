<script>
    import GridItem from '../../components/UI/GridItem.svelte';
    import GridLayout from '../../components/UI/GridLayout.svelte';

    import Content from '../../components/UI/Content.svelte';
    import Spacer from '../../components/UI/Spacer.svelte';

    import Navigation from '../../components/Styleguide/Navigation.svelte';

    // General
    let debug = false;

    // Styleguide related
    let styleguide = false;

</script>

<svelte:head>
	<title>Style guide</title>
</svelte:head>

<GridLayout>
    <GridItem>
        <Spacer side="top">
            <Content>
                <h3>Table of Contents</h3>
                <Navigation />
            </Content>
        </Spacer>
    </GridItem>
    <GridItem>
        <div id="components">
            <slot></slot>
        </div>
    </GridItem>
</GridLayout>