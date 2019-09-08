<style>

    .segmented-control {
        width: 100%;
        display: flex;
    }

    :global(.segmented-control li) {
        flex: 1 0 auto;
    }

</style>

<ul class="segmented-control">
    <slot></slot>
</ul>