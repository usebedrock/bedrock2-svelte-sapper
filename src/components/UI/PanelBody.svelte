<style>
    .panel-body {
       padding: 1.6rem;
    }

      .panel-body + .panel-body {
       border-top: 1px solid #DDD;
    }

    :global(.panel-nopad .panel-body) {
        padding: 1.6rem 0;
    }

    :global(.panel-minimal .panel-body + .panel-body) {
       border-top: 1px solid #EEE;
    }
</style>

 <div class="panel-body">
    <slot></slot>
</div>
