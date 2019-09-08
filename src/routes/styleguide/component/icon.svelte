<script>
    import Icon from '../../../components/UI/Icon.svelte';
    import Sample from '../../../components/Styleguide/Sample.svelte';
</script>

<style>

    .icon-list {
        display: flex;
    }

    .icon-list li {
        margin: 1rem;
    }
</style>

<Sample>
    <ul class="icon-list">
        <li><Icon icon="close" /></li>
        <li><Icon icon="add" /></li>
        <li><Icon icon="remove" /></li>
        <li><Icon icon="delete" /></li>
        <li><Icon icon="question" /></li>
        <li><Icon icon="menu" /></li>
        <li><Icon icon="chevron-left" /></li>
        <li><Icon icon="chevron-right" /></li>
    </ul>
</Sample>