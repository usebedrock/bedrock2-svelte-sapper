<script>
    export let id = null;
    export let value = null;
    export let changeEvent = null;
</script>

<style>
    select {
        -webkit-appearance: none;
        -moz-appearance: none;
        appearance: none;
        font-size: inherit;
        width: 100%;
        padding: 0.6rem 0.5rem;
        border-radius: 0.3rem;
        background: #FFF;
        border: 1px solid #BDBDBD;
    }

    .select-holder {
        position: relative;
        width: 100%;
        min-width: 8.5rem;
    }

    .select-holder:before,
    .select-holder:after {
        border-width: 1rem;
        border: 0.4rem solid #777;
        border-left-color: transparent;
        border-right-color: transparent;
        display: block;
        pointer-events: none;
        content: ' ';
        position: absolute;
        width: 0;
        height: 0;
        right: 1rem;
    }

    .select-holder:before {
        top: 0.7rem;
        border-top-color: transparent;
    }

    .select-holder:after {
        top: 1.8rem;
        border-bottom-color: transparent;
    }

    select:focus {
        outline: 0;
        border-color: #3A75CB;
        box-shadow: 0 0 0 0.1rem #3A75CB, 0 0 0 0.4rem #C3DCFF;
        transition: 0.1s ease-in-out all;
    }

</style>

<div class="select-holder">
    <select id={id} bind:value={value} on:change={changeEvent}>
        <slot></slot>
    </select>
</div>