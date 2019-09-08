<script>
import Content from '../components/UI/Content.svelte';

    let treeVisible = false;

    function toggleTree(e) {
        if (e.charCode == 13) {
            treeVisible = !treeVisible; 
        }
    }

</script>

<svelte:window on:keypress={toggleTree} />

<style>

    .page-tree {
        position: fixed;
        bottom: 0;
        right: 0;
        left: 0;
        background: #FFF;
        border-right: 1px solid #CCC;
        box-shadow: 0 0 0.5rem rgba(0,0,0,0.25);
        width: 300px;
        padding: 2rem;
        height: 100%;
    }

</style>

<slot></slot>

{#if treeVisible}
    <div class="page-tree">
        <Content>

            <h3>Prototype pages</h3>
            <p><a href="/styleguide">Styleguide</a></p>

            <h3>Prototype pages</h3>
            <ul>
                <!-- Please add your prototype pages here manually -->
                <li><a href="/">View 1</a></li>
            </ul>
        </Content>
    </div>
{/if}