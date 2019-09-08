<script>
    export let grow = null;
</script>

<style>

    :global(.toolbar-item) {
        flex: 0 1 auto;
        margin-right: 1.6rem;
    }

    :global(.toolbar-item:last-child) {
        margin-right: 0
    }

    :global(.toolbar-item h1) {
        margin: 0.8rem 0;
      font-size: 2.4rem;
      font-weight: 700;
    }

    :global(.toolbar-item.grow) {
        flex: 1 0 auto;
    }

</style>

 <div class="toolbar-item" class:grow={grow}>
    <slot></slot>
</div>