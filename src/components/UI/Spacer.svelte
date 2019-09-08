<script>
    export let side = null;

</script>
<style>
    .spacer {
        padding: 1.6rem;
    }

    .spacer-top {
        padding-top: 1.6rem;
    }
</style>

<div class="{side ? 'spacer-'+side : 'spacer'}">
    <slot></slot>
</div>