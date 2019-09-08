<script>
    import Content from '../../../components/UI/Content.svelte';
    import Alert from '../../../components/UI/Alert.svelte';
    import Sample from '../../../components/Styleguide/Sample.svelte';
</script>

<Content>

    <h3>Alert skins</h3>

    <h4>Default</h4>
    <Sample>
        <Alert type="default">I am a default alert.</Alert>
    </Sample>
    <h4>Error</h4>
    <Sample>
        <Alert type="error">I am an error message.</Alert>
    </Sample>
    <h4>Success</h4>
    <Sample>
        <Alert type="success">I am a success message.</Alert>
    </Sample>

    <h3>Alert types</h3>

    <h4>Normal</h4>
    <Sample>
        <Alert type="default">Hey, I don't have any options.</Alert>
    </Sample>
    <h4>Dismissible</h4>
    <Sample>
        <Alert type="default" dismissible>Hey, I am dismissible.</Alert>
    </Sample>

</Content>