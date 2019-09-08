<script>
    import Content from '../../../components/UI/Content.svelte';
    import Sample from '../../../components/Styleguide/Sample.svelte';
    import Pre from '../../../components/UI/Pre.svelte';

    import Label from '../../../components/UI/Label.svelte';
    import Input from '../../../components/UI/Input.svelte';

    import FormGroup from '../../../components/UI/FormGroup.svelte';
    import FormGroupLayout from '../../../components/UI/FormGroupLayout.svelte';
</script>

<Content>
    <h3>Standard</h3>
</Content>

<Sample>
    <FormGroupLayout>
        <FormGroup>
            <Label>Field name</Label>
            <Input value="Value" />
        </FormGroup>
        <FormGroup>
            <Label>Field name</Label>
            <Input value="Value" />
        </FormGroup>
        <FormGroup>
            <Label>Field name</Label>
            <Input value="Value" />
        </FormGroup>
    </FormGroupLayout>
</Sample>

<Content>
    <h3>Horizontal</h3>
</Content>

<Sample>
    <FormGroupLayout type="horizontal">
        <FormGroup>
            <Label>Field name</Label>
            <Input value="Value" />
        </FormGroup>
        <FormGroup>
            <Label>Field name</Label>
            <Input value="Value" />
        </FormGroup>
        <FormGroup>
            <Label>Field name</Label>
            <Input value="Value" />
        </FormGroup>
    </FormGroupLayout>
</Sample>