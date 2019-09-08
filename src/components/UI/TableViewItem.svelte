<script>

    import Icon from './Icon.svelte';

    export let href;

</script>

<style>

    .table-view-item a {
        display: block;
        padding: 1.6rem;
        border-bottom: 1px solid #CCC;
        text-decoration: none;
        color: #000;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

</style>

<li class="table-view-item">
    <a href="{href}">
        <div>
            <slot></slot>
        </div>
        <Icon icon="chevron-right" />
    </a>
</li>