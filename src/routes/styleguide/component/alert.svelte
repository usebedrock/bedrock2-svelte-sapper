<script>

    import Prism from 'svelte-prism';

    import Content from '../../../components/UI/Content.svelte';
    import Alert from '../../../components/UI/Alert.svelte';
    import Sample from '../../../components/Styleguide/Sample.svelte';

    const defaultAlert = '<Alert type="default">I am a default alert.</Alert>';
    const errorAlert = '<Alert type="error">I am an error message.</Alert>';
    const successAlert = '<Alert type="success">I am a success message.</Alert>';
    const alertTypeDefault = '<Alert type="default">Hey, I don\'t have any options.</Alert>';
    const alertTypeDismissible = '<Alert type="default" dismissible>Hey, I am dismissible.</Alert>';

</script>

<Content>

    <h2>Alert skins</h2>

    <h3>Default</h3>
    <Sample>
        <Alert type="default">I am a default alert.</Alert>
    </Sample>
    <Prism language="html" source="{defaultAlert}" />

    <h3>Error</h3>
    <Sample>
        <Alert type="error">I am an error message.</Alert>
    </Sample>
    <Prism language="html" source="{errorAlert}" />


    <h3>Success</h3>
    <Sample>
        <Alert type="success">I am a success message.</Alert>
    </Sample>
    <Prism language="html" source="{errorAlert}" />

    <h2>Alert types</h2>

    <h3>Normal</h3>
    <Sample>
        <Alert type="default">Hey, I don't have any options.</Alert>
    </Sample>
    <Prism language="html" source="{alertTypeDefault}" />

    <h3>Dismissible</h3>
    <Sample>
        <Alert type="default" dismissible>Hey, I am dismissible.</Alert>
    </Sample>
    <Prism language="html" source="{alertTypeDismissible}" />

</Content>

