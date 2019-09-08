<script>
    import Pre from '../../../components/UI/Pre.svelte';
    import Code from '../../../components/UI/Code.svelte';
    import Content from '../../../components/UI/Content.svelte';

    let stringShort = 'Excepteur sint occaecat cupidatat non proident';
    let stringMedium = 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.';

    let styles = [
        {
            size: '28',
            name: "Heading 1",
            previewString: "<h1>Heading 1</h1>"
        },
        {
            size: '22',
            name: "Heading 2",
            previewString: "<h2>Heading 2</h2>"
        },
        {
            size: '18',
            name: "Heading 3",
            previewString: "<h3>Heading 3</h3>"
        },
        {
            size: '14',
            name: "Body 1",
            previewString:  "<p>"+stringMedium+"</p>"
        },
        {
            size: '12',
            name: "Body 2",
            previewString: "<p class='c-body-2'>"+stringShort+"</p>"
        },
    ]
</script>

<table class="table">
    <thead>
        <tr>
            <th>Name</th>
            <th>Preview</th>
        </tr>
    </thead>
    <tbody>
    {#each styles as style}
        <tr>
            <td>
                {style.name}
                <br>
                {style.size}px
            </td>

            <td>
                <Content>
                    {@html style.previewString}
                </Content>
            </td>
            
        </tr>
    {/each}
    </tbody>
</table>