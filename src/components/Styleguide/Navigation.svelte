<script>

    export let segment;

    let componentTreeCategories = ["Basics", "Atoms", "Components", "Objects"];

    let componentTree = [
        {
            category: "Atoms",
            name: "Button",
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
            category: "Components",
            name: "Segmented control"
        },
        {
            category: "Components",
            name: "Table view"
        },
        {
            category: "Components",
            name: "Card"
        },
        {
            category: "Components",
            name: "Alert"
        },
        {
            category: "Components",
            name: "Box"
        },
        {
            category: "Atoms",
            name: "Input"
        },
        {
            category: "Basics",
            name: "Icon"
        },
        {
            category: "Components",
            name: "Blank slate"
        },
        {
            category: "Components",
            name: "Panel"
        },
        {
            category: "Objects",
            name: "Form group"
        },
        {
            category: "Components",
            name: "Toolbar"
        },
        {
            category: "Components",
            name: "Select"
        }
    ];

</script>

<style>
    h4 {
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

    .selected {
        background: red;
    }
</style>

<ul>
    {#each componentTreeCategories as componentTreeCategory}
        <li>
            <h4>{componentTreeCategory}</h4>
            <ul>
                {#each componentTree as component}
                    {#if component.category == componentTreeCategory }
                        <li
                            class:selected={ segment === component.name.trim().toLowerCase().replace(" ", "-")}
                        >
                            <!-- to debug selected state -->
                            <!-- {segment}
                            {component.name.trim().toLowerCase().replace(" ", "-")} -->
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