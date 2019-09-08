<script>

    import ButtonInnerLayout from './ButtonInnerLayout.svelte';

    // a link, type="button" or type="submit"
    export let type = false;

    // Extra class
    export let classValue = null;

    // if it contains a link
    export let href = false;

    // Value
    export let value = "Default value";

    // Disabled
    export let disabled = false;

    // Styling
    export let style = null;
    export let icon = null;
    export let layout = null;
    export let variant = null;

</script>

<style>

    a, button {
        font-size: 1.4rem;
    }

    button {
        font-family: var(--base-font);
    }

    a {
        text-decoration: none;
    }

    a, button {
        background: #F0F0F0;
        border: 1px solid #CCC;
        border-radius: 0.3rem;
        padding: 0.7rem;
        align-items: center;
        display: inline-flex;
        justify-content: center;
        vertical-align: baseline;
        color: #333;
        white-space: nowrap;
    }

    button[disabled] {
        opacity: 0.4;
    }

    a:focus, button:focus {
        background: #FFF;
        outline: 0;
        border-color: #3A75CB;
        box-shadow: 0 0 0 0.1rem #3A75CB, 0 0 0 0.4rem #C3DCFF;
        transition: 0.1s ease-in-out all;
    }

    .primary {
        background: #748DD5;
        border-color: #748DD5;
        color: #FFF; 
    }

    .success {
        background: #75D37E;
        border-color: #75D37E;
        color: #FFF;
    }

</style>

<!--
    @todo de-duplicate some logic here
    @see discussion around classNames package
-->

{#if href}
   <a
    href="{href}"
    {style}
    {classValue}
    class:primary={variant==='primary'}
    class:success={variant==='success'}
  >
        <ButtonInnerLayout {icon} {layout}><slot></slot></ButtonInnerLayout>
   </a>
{:else}
    {#if type == "submit"}
        <button
            type="submit"
            {disabled}
            {classValue}
            {style}
            class:primary={variant==='primary'}
            class:success={variant==='success'}
            on:submit on:click
        >
            <ButtonInnerLayout {icon} {layout}><slot></slot></ButtonInnerLayout>
        </button>
    {:else}
        <button
            type="button"
            {disabled}
            {classValue}
            {style}
            on:submit|preventDefault on:click
            class:primary={variant==='primary'}
            class:success={variant==='success'}
        >
            <ButtonInnerLayout {icon} {layout}><slot></slot></ButtonInnerLayout>
        </button>
    {/if}
{/if}
