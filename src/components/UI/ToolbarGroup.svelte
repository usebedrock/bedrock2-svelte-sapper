<script>
    export let align;
</script>

<style>

     :global(.toolbar-group) {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }


    :global(.toolbar-group-justify) { width: 100%; }
    :global(.toolbar-group-left) { order: 1; }
    :global(.toolbar-group-center) { order: 2; }
    :global(.toolbar-group-right) { order: 3; }


</style>

 <div
    class="toolbar-group"
    class:toolbar-group-left={align==='left'}
    class:toolbar-group-center={align==='center'}
    class:toolbar-group-right={align==='right'}
    class:toolbar-group-justify={align==='justify'}
>
    <slot></slot>
</div>