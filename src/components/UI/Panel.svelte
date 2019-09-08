<script>
    export let minimal = false;
    export let ghost = false;
    export let nopad = false;
</script>

<style>
    .panel {
        border: 1px solid #DDD;
        background: #FFF;
        border-radius: 0.4rem;
    }

   .panel-minimal {
        border: 1px solid #EEE;
        background: #FFF;
    }

    .panel-ghost {
        border: 1px solid transparent;
        background: transparent;
    }

</style>

 <div class="panel {minimal ? 'panel-minimal' : ''} {nopad ? 'panel-nopad' : ''} {ghost ? 'panel-ghost' : ''}">
    <slot></slot>
</div>
