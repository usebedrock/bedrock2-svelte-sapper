<script>
    import Sample from '../../../components/Styleguide/Sample.svelte';

    import SegmentedControl from '../../../components/UI/SegmentedControl.svelte';
    import SegmentedControlItem from '../../../components/UI/SegmentedControlItem.svelte';
</script>

<Sample>
    <SegmentedControl>
        <SegmentedControlItem active href="/">Tab 1</SegmentedControlItem>
        <SegmentedControlItem href="/">Tab 2</SegmentedControlItem>
        <SegmentedControlItem href="/">Tab 3</SegmentedControlItem>
        <SegmentedControlItem href="/">Tab 4</SegmentedControlItem>
    </SegmentedControl>
</Sample>