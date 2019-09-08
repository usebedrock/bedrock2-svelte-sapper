<script>
    export let href;
    export let active;
</script>
<style>

    .segmented-control-item a {
        display: block;
        padding: 0.8rem;
        text-align: center;
        text-decoration: none;
        color: #333;
        background: #EEE;
        border: 1px solid #DDD;
    }

    .segmented-control-item.active a {
        background: #FFF
    }

    .segmented-control-item + .segmented-control-item a {
        border-left: none;
    }
</style>

<li class="segmented-control-item" class:active={active}>
    <a href="{href}">
        <slot></slot>
    </a>
</li>