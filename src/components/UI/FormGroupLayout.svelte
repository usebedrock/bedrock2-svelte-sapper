<script>
    export let type = "standard";
</script>

<style>

    :global(.form-group-layout-horizontal .form-group) {
        display: flex;
    }

    :global(.form-group-layout-horizontal .form-group-controls) {
        flex: 1 1 auto;
    }

    :global(.form-group-layout-inline .form-group) {
        display: flex;
        align-items: center;
    }

</style>

{#if type == "standard"}
    <div class="form-group-layout-standard">
        <slot></slot>
    </div>
{:else if type == "horizontal" }
    <div class="form-group-layout-horizontal">
        <slot></slot>
    </div>
{:else if type == "inline" }
    <div class="form-group-layout-inline">
        <slot></slot>
    </div>
{/if}