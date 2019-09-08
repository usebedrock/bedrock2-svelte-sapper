<script>

    export let segment;

    let componentTreeCategories = ["Basics", "Atoms", "Components"];

    let componentTree = [
        {
            category: "Atoms",
            name: "Button",
        },
        {
            category: "Atoms",
            name: "Input"
        },
        {
            category: "Basics",
            name: "Colors",
        },
        {
            category: "Basics",
            name: "Typography",
        },
        {
            category: "Basics",
            name: "Icon"
        },
        {
            category: "Components",
            name: "Alert"
        },
        {
            category: "Components",
            name: "Blank slate"
        },
        {
            category: "Components",
            name: "Box"
        },
        {
            category: "Components",
            name: "Content"
        },
        {
            category: "Components",
            name: "Card"
        },
        {
            category: "Components",
            name: "Segmented control"
        },
        {
            category: "Components",
            name: "Table view"
        },
        {
            category: "Components",
            name: "Panel"
        },
        {
            category: "Components",
            name: "Form group"
        },
        {
            category: "Components",
            name: "Toolbar"
        },
        {
            category: "Components",
            name: "Select"
        },
        {
            category: "Components",
            name: "Table"
        }
    ];

</script>

<style>
    h2 {
        margin: 1rem 0;
    }

    ul {
        padding: 0 0 1.2rem;
    }

    a {
        color: #000;
        text-decoration: none;
        display: block;
        padding: 0.8rem;
    }

    a:hover {
        background: #EEE;
    }

    ul li {
        list-style: none;
    }
</style>

<nav>
    <ul>
        {#each componentTreeCategories as componentTreeCategory}
            <li>
                <h2 class="c-h4">{componentTreeCategory}</h2>
                <ul>
                    {#each componentTree as component}
                        {#if component.category == componentTreeCategory }
                            <li>
                                <a href={'/styleguide/component/'+component.name.trim().toLowerCase().replace(" ", "-")}>
                                    {component.name}
                                </a>
                            </li>
                        {/if}
                    {/each}
                </ul>
            </li>
        {/each}
    </ul>
</nav>