<script>
    import Sample from '../../../components/Styleguide/Sample.svelte';
    import Content from '../../../components/UI/Content.svelte';
    import Code from '../../../components/UI/Code.svelte';
    import Pre from '../../../components/UI/Pre.svelte';
</script>

<Content>
    <p>Use the <Code>Content</Code> component to style rich text.</p>
    <p>You can use certain CSS classes to style tags directly without needing this component.</p>
</Content>

<Sample>
    <Content>
        <h2>Hello world</h2>
        <p>Hey, I am a paragraph.</p>
        <ul>
            <li>Bullet 1</li>
            <li>Bullet 2</li>
            <li>Bullet 3</li>
        </ul>
         <ol>
            <li>Ordered list item 1</li>
            <li>Ordered list item 2</li>
            <li>Ordered list item 3</li>
        </ol>
    </Content>
</Sample>