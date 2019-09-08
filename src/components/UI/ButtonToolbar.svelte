<style>
    .button-toolbar {
        display: flex;
        flex-wrap: wrap;
    }

    :global(.button-toolbar button) {
        margin-right: 0.5rem;
        margin-bottom: 0.5rem;
    }

    :global(.button-toolbar button:last-child) {
        margin-right: 0;
    }
</style>

 <div class="button-toolbar">
    <slot></slot>
</div>