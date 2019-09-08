<script>
    import Content from '../../../components/UI/Content.svelte';
    import Button from '../../../components/UI/Button.svelte';
    import Sample from '../../../components/Styleguide/Sample.svelte';
</script>

<Content>
    <h2>Button skins</h2>

    <Sample>
        <Button variant="primary">Button label</Button>
        <Button variant="success">Button label</Button>
    </Sample>

    <h2>Button types</h2>

    <h3>Icon only</h3>
    <Sample>
        <Button icon="close" layout="icon-only">Close</Button>
    </Sample>

    <h3>Regular (action button)</h3>

    <Sample>
        <Button>Hello</Button>
    </Sample>

    <h3>Link</h3>

    <p>Use a <code>href</code> attribute.</p>

    <Sample>
        <Button href="/">Hello</Button>
    </Sample>

    <h3>Icon and label</h3>

    <Sample>
        <Button icon="close">Close</Button>
        <Button icon="add">Add</Button>
        <Button icon="remove">Remove</Button>
        <Button icon="delete">Delete</Button>
        <Button icon="question">Help</Button>
    </Sample>
</Content>