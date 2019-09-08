<script>
    import Content from '../../../components/UI/Content.svelte';
    import Sample from '../../../components/Styleguide/Sample.svelte';

    import Label from '../../../components/UI/Label.svelte';
    import Input from '../../../components/UI/Input.svelte';
    import InputColor from '../../../components/UI/InputColor.svelte';
    import InputNumber from '../../../components/UI/InputNumber.svelte';
</script>

<Content>
    <h2>Inputs</h2>

    <h3>Text</h3>

    <Sample>
        <Input value="Test" />
    </Sample>

    <h3>Color</h3>
    <Sample>
        <InputColor value="#FF0000" />
    </Sample>

    <!-- todo input number example -->
</Content>