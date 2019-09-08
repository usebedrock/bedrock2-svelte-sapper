<script>
    import Sample from '../../../components/Styleguide/Sample.svelte';

    import Card from '../../../components/UI/Card.svelte';
    import CardList from '../../../components/UI/CardList.svelte';
    import Pre from '../../../components/UI/Pre.svelte';
</script>

<Sample>
    <Card>
        <p>I am card content</p>
    </Card>
</Sample>

<Pre>&lt;Card&gt;
    &lt;p&gt;I am card content&lt;/p&gt;
&lt;/Card&gt;</Pre>

<Sample>
    <Card href="/">
        <p>I am card content with a link</p>
    </Card>
</Sample>

<Pre>&lt;Card href=&quot;/&quot;&gt;
    &lt;p&gt;I am card content with a link&lt;/p&gt;
&lt;/Card&gt;</Pre>