<script>
    export let segment
    import Intro from './_intro.svelte';
</script>

<Intro segment={segment} />

<slot></slot>
