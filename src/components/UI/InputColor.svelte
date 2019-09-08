<script>
    export let id = null;
    export let value = null;
    export let style = null;
</script>

<style>

    input[type="color"] {
        border: none;
        border-radius: 0.3rem;
        height: 1.6rem;
        width: 1.6rem;
        min-height: 2rem;
        line-height: 2rem;
        min-width: 2rem;
        padding: 0;
    }

    input[type="color"]:focus {
        outline: 0;
        border-color: #3A75CB;
        box-shadow: 0 0 0 0.1rem #3A75CB, 0 0 0 0.4rem #C3DCFF;
        transition: 0.1s ease-in-out all;
    }

</style>

<input type="color" {id} bind:value={value} {style}>