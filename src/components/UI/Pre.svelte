<script>
    import Button from './Button.svelte';

    let showCode = false;

    function toggleCode() {
        showCode = !showCode;
    }
</script>

<style>

    :global(.pre-holder button) {
        margin: 0 0 1.2rem;
    }

    pre {
        background: #F0F0F0;
        font-family: monospace;
        padding: 1.4rem;
        margin: 0 0 2rem;
    }

    code {
        color: red;
    }

</style>

<div class="pre-holder">
    <Button on:click={toggleCode}>Show code</Button>
    {#if showCode}
        <pre><code><slot></slot></code></pre>
    {/if}
</div>