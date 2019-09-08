<script>

    import Icon from './Icon.svelte';

    export let href = null;

</script>

<style>
    .card {
        border: 1px solid #DDD;
        background: #F0F0F0;
        border-radius: 0.4rem;
        padding: 1.6rem;
    }

    .card-is-link {
        padding: 0;
    }

    .card a {
        display: block;
        padding: 1.6rem;
        text-decoration: none;
        color: #000;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
</style>

<div class="card" class:card-is-link={href}>
    {#if href}
        <a href="{href}">
            <div>
                <slot></slot>
            </div>
            <Icon icon="chevron-right" />
        </a>
    {:else}
        <slot></slot>
    {/if}
</div>