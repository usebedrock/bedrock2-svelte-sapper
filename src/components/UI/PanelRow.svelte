<script>
    export let panelCount;
</script>
<style>

    :global(.panel-row  > .panel) {
        margin-bottom: 2rem;
    }

    @media (min-width: 1024px) {

        .panel-row  {
            display: flex;
        }

        :global(.panel-row  > .panel) {
            flex: 0 1 33.3333%;
            margin-right: 2rem;
        }

        :global(.panel-row-2  > .panel) {
            flex: 0 1 50%;
            margin-right: 2rem;
        }

        :global(.panel-row  > .panel:last-child) {
            margin-right: 0;
        }

    }
</style>

{#if panelCount = 2 }
 <div class="panel-row panel-row-2">
    <slot></slot>
  </div>
{:else}
 <div class="panel-row">
    <slot></slot>
  </div>
{/if}




