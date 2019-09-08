<script>
    export let segment
    import Intro from './_Intro.svelte';
</script>

<Intro segment={segment} />

<slot></slot>
