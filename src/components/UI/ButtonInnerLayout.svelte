<script>
    import Icon from './Icon.svelte';

    // layouts: icon-only, label-icon, icon-label, icon-label-icon, icon-label-narrow-icon
    export let layout = "label";

    export let icon = null;
    export let icon2 = null;

</script>

<style>
    .button-label {
        margin-left: 0.4rem;
    }
    .icon-only-wrap {
        display: flex;
        align-items: center;
        padding-left: 0.6rem;
        padding-right: 0.6rem;
    }
</style>

{#if layout == "icon-only"}
    <span class="icon-only-wrap"><Icon {icon} /></span>
    <span class="u-sr-only"><slot></slot></span>
{:else if layout == "icon-label-icon"}
    <Icon {icon} />
    <span class="button-label"><slot></slot></span>
    <Icon icon={icon2} />
{:else if icon}
    <Icon {icon} />
    <span class="button-label"><slot></slot></span>
{:else}
    <span class="button-label"><slot></slot></span>
{/if}
