<script>
    import Pre from '../../../components/UI/Pre.svelte';
    import Sample from '../../../components/Styleguide/Sample.svelte';
    import Code from '../../../components/UI/Code.svelte';
    import Content from '../../../components/UI/Content.svelte';
</script>

<Content>
    <p>To implement a styled table, simply add a <Code>.table</Code> class to an HTML table.</p>
</Content>

<Sample>
    <table class="table">
        <thead>
            <th>Header</th>
            <th>Header</th>
            <th>Header</th>
            <th>Header</th>
        </thead>
        <tbody>
            <tr>
                <td>Data</td>
                <td>Data</td>
                <td>Data</td>
                <td>Data</td>
            </tr>
            <tr>
                <td>Data</td>
                <td>Data</td>
                <td>Data</td>
                <td>Data</td>
            </tr>
        </tbody>
    </table>
</Sample>