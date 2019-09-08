<script>
    import Content from '../../../components/UI/Content.svelte';
    import Sample from '../../../components/Styleguide/Sample.svelte';

    import Panel from '../../../components/UI/Panel.svelte';
    import PanelBody from '../../../components/UI/PanelBody.svelte';
    import PanelHeader from '../../../components/UI/PanelHeader.svelte';
    import PanelRow from '../../../components/UI/PanelRow.svelte';

</script>

<Content>
    <p>Use panels to easily create layouts.</p>
</Content>

<Sample>
    <Panel>
        <PanelHeader title="Panel header" />
        <PanelBody>
            <p>I am HTML content.</p>
        </PanelBody>
    </Panel>
</Sample>

<Sample>
    <PanelRow panelCount="2'">
        <Panel>
            <PanelHeader title="Panel header" />
            <PanelBody>
                <p>I am HTML content.</p>
            </PanelBody>
        </Panel>
        <Panel>
            <PanelHeader title="Panel header" />
            <PanelBody>
                <p>I am HTML content.</p>
            </PanelBody>
        </Panel>
    </PanelRow>
</Sample>
<Sample>
    <PanelRow>
        <Panel>
            <PanelHeader title="Panel header" />
            <PanelBody>
                <p>I am HTML content.</p>
            </PanelBody>
        </Panel>
        <Panel>
            <PanelHeader title="Panel header" />
            <PanelBody>
                <p>I am HTML content.</p>
            </PanelBody>
        </Panel>
        <Panel>
            <PanelHeader title="Panel header" />
            <PanelBody>
                <p>I am HTML content.</p>
            </PanelBody>
        </Panel>
    </PanelRow>
</Sample>