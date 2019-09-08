<script>
    export let forValue = null;
</script>
<style>

    label {
        display: block;
        font-weight: 700;
        margin: 0 0 0.4rem;
    }

    :global(.form-group-layout-horizontal label) {
        margin-top: 0.6rem;
        min-width: 12rem;
    }

    :global(.form-group-layout-horizontal .form-group label) {
        flex: 0 1 12rem;
    }

    :global(.form-group-layout-inline .form-group label) {
        margin-right: 1.2rem;
        white-space: nowrap;
    }

</style>

<label for="{forValue}">
    <slot></slot>
</label>
