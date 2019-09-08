<script>
    import Content from '../UI/Content.svelte';

    export let name = null;
    export let description = null;

    let nameId;

    $: nameId = name.trim().toLowerCase().replace(" ", "-");
</script>

<style>

    .component {
        border-bottom: 1px solid #CCC;
        padding: 0 0 3.6rem;
        margin: 0 0  3.6rem;
    }

</style>

<div class="component" id="{nameId}">
    {#if name}
        <h3 class="c-h3">{name}</h3>
    {/if}
    {#if description}
        <Content>
            <p>{description}</p>
        </Content>
    {/if}
    <slot></slot>
</div>