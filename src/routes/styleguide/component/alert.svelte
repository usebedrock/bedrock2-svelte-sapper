<script>
    import Content from '../../../components/UI/Content.svelte';
    import Alert from '../../../components/UI/Alert.svelte';
    import Sample from '../../../components/Styleguide/Sample.svelte';
</script>

<Content>

    <h2>Alert skins</h2>

    <h3>Default</h3>
    <Sample>
        <Alert type="default">I am a default alert.</Alert>
    </Sample>
    <h3>Error</h3>
    <Sample>
        <Alert type="error">I am an error message.</Alert>
    </Sample>
    <h3>Success</h3>
    <Sample>
        <Alert type="success">I am a success message.</Alert>
    </Sample>

    <h2>Alert types</h2>

    <h3>Normal</h3>
    <Sample>
        <Alert type="default">Hey, I don't have any options.</Alert>
    </Sample>
    <h3>Dismissible</h3>
    <Sample>
        <Alert type="default" dismissible>Hey, I am dismissible.</Alert>
    </Sample>

</Content>