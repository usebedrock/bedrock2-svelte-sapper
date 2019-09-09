## Bedrock 2

Welcome to Bedrock. Bedrock is a prototyping environment to quickly build user interfaces.

Main features include:

* Style guide ("design system"): documentation of the components that are available to you
* Page tree: view the pages in your prototype in a handy side panel

## Create a Bedrock 2 based prototype

We recommend using `degit` to be able to grab a Bedrock install without actually cloning the project repository. Degit is a way of cloning a repository without including the Git folder.

Here is the series of commands you can use to start a new prototype:

    npm i -g degit
    degit usebedrock/bedrock2 my-bedrock-2-project
    cd my-bedrock-2-project/
    npm install
    npm run dev

Now visit `http://localhost:3000` to view your project.

## Export your results

The way to export your resulting project is to run:

    npm run export

Your generated website will live in a folder called `__sapper__/export`.

## Development on Bedrock 2 itself

To run the project:

    npm install
    npm run dev

## How to contribute



## Requirements

* Node LTS
