<script>
    import Code from '../../../components/UI/Code.svelte';

    let colors = [
        {
            hex: '#CCC',
            name: "Border",
            category: "Semantic",
            variable: "--color-semantic-border"
        },
        {
            hex: '#FFC',
            name: "Highlight",
            category: "Semantic",
            variable: "--color-yellow"
        },
        {
            hex: '#758FD3',
            name: "Success",
            category: "Semantic",
            variable: "--color-semantic-primary"
        },
        {
            hex: '#75D37E',
            name: "Primary",
            category: "Semantic",
            variable: "--color-semantic-success"
        },
    ]
</script>

<style>
    .color-example {
        width: 4rem;
        height: 4rem;
    }

</style>

<table class="table">
    <thead>
        <tr>
            <th>Preview</th>
            <th>Category</th>
            <th>Name</th>
            <th>Variable</th>
        </tr>
    </thead>
    <tbody>
    {#each colors as color}
        <tr>
            <td><div class="color-example" style="background: {color.hex};"></div></td>
            <td>{color.category}</td>
            <td>{color.name}</td>
            <td><Code>{color.variable}</Code></td>
        </tr>
    {/each}
    </tbody>
</table>