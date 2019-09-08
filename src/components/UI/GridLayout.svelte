<script>
    export let columns = 2;
</script>

<style>

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