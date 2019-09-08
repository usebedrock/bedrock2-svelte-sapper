<script>
    export let columns = 2;
</script>

<style>

    /* This code works for a specific layout at this point in time, not a generic grid component yet. */
    .grid-layout {
        display: grid;
        grid-gap: 2rem;
        grid-template-columns: 30rem minmax(30rem, 1fr);
        height: 100%;
    }

</style>

<div class="grid-layout">
    <slot></slot>
</div>