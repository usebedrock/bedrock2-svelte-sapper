<script>

    import Content from '../../../components/UI/Content.svelte';

    export let segment;
    $: segment = segment.replace("-", " ").replace(/^\w/, c => c.toUpperCase());

</script>

<Content>
    <h2>{segment}</h2>
</Content>

<!-- @todo implement component descriptions -->
<!-- <p>Component description</p> -->