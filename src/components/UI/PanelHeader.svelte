<script>
  export let title;
</script>

<style>
    .panel-header {
       border-bottom: 1px solid #DDD;
       padding: 0.8rem 1.6rem;
    }

    :global(.panel-minimal .panel-header) {
       border-bottom: 1px solid #EEE;
    }

    :global(.panel-nopad .panel-header) {
        padding: 0.8rem 0;
    }

    h3 {
        margin: 0.8rem 0;
        font-size: 1.8rem;
        font-weight: 700;
    }
</style>

<div class="panel-header">
    <slot name="panel-header">
        <h3>{title}</h3>
    </slot>
</div>
