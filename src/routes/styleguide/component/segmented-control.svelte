<script>
    import Sample from '../../../components/Styleguide/Sample.svelte';
    import Pre from '../../../components/UI/Pre.svelte';

    import SegmentedControl from '../../../components/UI/SegmentedControl.svelte';
    import SegmentedControlItem from '../../../components/UI/SegmentedControlItem.svelte';
</script>

<Sample>
    <SegmentedControl>
        <SegmentedControlItem active href="/">Tab 1</SegmentedControlItem>
        <SegmentedControlItem href="/">Tab 2</SegmentedControlItem>
        <SegmentedControlItem href="/">Tab 3</SegmentedControlItem>
    </SegmentedControl>
</Sample>

<Pre>&lt;SegmentedControl&gt;
    &lt;SegmentedControlItem active href=&quot;/&quot;&gt;Tab 1&lt;/SegmentedControlItem&gt;
    &lt;SegmentedControlItem href=&quot;/&quot;&gt;Tab 2&lt;/SegmentedControlItem&gt;
    &lt;SegmentedControlItem href=&quot;/&quot;&gt;Tab 3&lt;/SegmentedControlItem&gt;
&lt;/SegmentedControl&gt;</Pre>