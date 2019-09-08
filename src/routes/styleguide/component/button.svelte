<script>
    import Content from '../../../components/UI/Content.svelte';
    import Button from '../../../components/UI/Button.svelte';
    import Sample from '../../../components/Styleguide/Sample.svelte';
</script>

<Content>
    <h3>Button skins</h3>

    <Sample>
        <Button variant="primary">Button label</Button>
        <Button variant="success">Button label</Button>
    </Sample>

    <h3>Button types</h3>

    <h4>Icon only</h4>
    <Sample>
        <Button icon="close" layout="icon-only">Close</Button>
    </Sample>

    <h4>Regular (action button)</h4>

    <Sample>
        <Button>Hello</Button>
    </Sample>

    <h4>Link</h4>

    <p>Use a <code>href</code> attribute.</p>

    <Sample>
        <Button>Hello</Button>
    </Sample>

    <h4>Icon and label</h4>
    <Sample>
        <Button icon="close">Close</Button>
        <Button icon="add">Add</Button>
        <Button icon="remove">Remove</Button>
        <Button icon="delete">Delete</Button>
        <Button icon="question">Help</Button>
    </Sample>
</Content>