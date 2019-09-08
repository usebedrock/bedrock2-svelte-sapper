<script>
    export let id = null;
    export let value = '';
    export let type = "text";
    export let disabled = false;
    export let labelId = null;
</script>

<style>

    input {
        font-size: 1.4rem;
        line-height: 1.3;
        font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
        width: 100%;
        padding: 0.6rem;
        background: #FFF;
        color: #333;
        border-radius: 0.3rem;
        border: 1px solid #BDBDBD;
        box-shadow: inset 0.1rem 0.1rem 0.2rem 0 rgba(0,0,0,0.12);
    }

    input:focus {
        outline: 0;
        border-color: #3A75CB;
        box-shadow: 0 0 0 0.1rem #3A75CB, 0 0 0 0.4rem #C3DCFF;
        transition: 0.1s ease-in-out all;
    }

    input[disabled] {
        background: #EEE;
    }

</style>

{#if type == "password" }
    <input id={labelId ? labelId : id} type="password" bind:value={value} {disabled}>
{:else}
    <input id={labelId ? labelId : id} type="text" bind:value={value} {disabled}>
{/if}
