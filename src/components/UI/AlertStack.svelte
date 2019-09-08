<script>

    import { beforeUpdate } from 'svelte';
    import Alert from './Alert.svelte';
    export let alertStackData = ['Message', 'Message', 'Message'];

    function removeDuplicates(names) {
        let unique = {};
        names.forEach(function(i) {
            if(!unique[i]) {
                unique[i] = true;
            }
        });
       return Object.keys(unique);
    }

    $: alertStackData = removeDuplicates(alertStackData);

</script>

<style>

    .alert-stack {
        position: fixed;
        bottom: 1.2rem;
        right: 1.2rem;
        list-style: none;
    }

    .alert-stack li {
        padding-top: 12px;
    }

</style>

{#if alertStackData}
    <ul class="alert-stack">
        {#each alertStackData as item}
            <li>
                <Alert type="error">{item}</Alert>
            </li>
        {/each}
    </ul>
{/if}