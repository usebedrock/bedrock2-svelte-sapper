<script>
    export let id;
    export let value;
    export let max;
    export let min;
    export let style;
    export let classValue;
</script>

<style>

    input[type="number"] {
        width: 100%;
        padding: 0.5rem;
        background: #FFF;
        border-radius: 0.3rem;
        border: 1px solid #BDBDBD;
        box-shadow: inset 0.1rem 0.1rem 0.2rem 0 rgba(0,0,0,0.12);
    }

    /* Improve with invalid styles */
    /* class:invalid={!isValidNumber(skillMapNumber)} */

</style>

<input type="number" {id} bind:value={value} {max} {min} {style} class="{classValue}">