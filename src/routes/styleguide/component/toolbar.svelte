<script>
    import Sample from '../../../components/Styleguide/Sample.svelte';

    import Button from '../../../components/UI/Button.svelte';

    import Toolbar from '../../../components/UI/Toolbar.svelte';
    import ToolbarGroup from '../../../components/UI/ToolbarGroup.svelte';
    import ToolbarItem from '../../../components/UI/ToolbarItem.svelte';
    import ToolbarTitle from '../../../components/UI/ToolbarTitle.svelte';

</script>

<Sample>
    <Toolbar>
        <ToolbarGroup>
            <ToolbarItem>
                <ToolbarTitle>Toolbar title</ToolbarTitle>
            </ToolbarItem>
        </ToolbarGroup>
        <ToolbarGroup>
            <ToolbarItem>
                <Button>Button label</Button>
            </ToolbarItem>
            <ToolbarItem>
                <Button>Button label</Button>
            </ToolbarItem>
            <ToolbarItem>
                <Button>Button label</Button>
            </ToolbarItem>
        </ToolbarGroup>
    </Toolbar>
</Sample>

<Sample>
    <Toolbar>
        <ToolbarGroup align="left">
            <ToolbarItem>
                <Button>Button label</Button>
            </ToolbarItem>
        </ToolbarGroup>
        <ToolbarGroup align="center">
            <ToolbarItem>
                <ToolbarTitle>Toolbar title</ToolbarTitle>
            </ToolbarItem>
        </ToolbarGroup>
        <ToolbarGroup align="right">
            <ToolbarItem>
                <Button>Button label</Button>
            </ToolbarItem>
        </ToolbarGroup>
    </Toolbar>
</Sample>


<Sample>
    <Toolbar>
        <!-- You might leave an empty toolbar group for spacing -->
        <ToolbarGroup align="left">
        </ToolbarGroup>
        <ToolbarGroup align="center">
            <ToolbarItem>
                <ToolbarTitle>Toolbar title</ToolbarTitle>
            </ToolbarItem>
        </ToolbarGroup>
        <ToolbarGroup align="right">
            <ToolbarItem>
                <Button>Button label</Button>
            </ToolbarItem>
        </ToolbarGroup>
    </Toolbar>
</Sample>

