# example-node

[![view-action-graph](https://img.shields.io/github/actions/workflow/status/actionforge/example-node/workflow.yml?label=View%20Action%20Graph)](https://app.actionforge.dev/github/actionforge/example-node/main/.github/workflows/graphs/build.act)

A simple Hello World app in Node.js, built using an [Actionforge](https://actionforge.dev) graph as the CI/CD pipeline.

## Run

```bash
node index.js
```

## Graph

The build pipeline is defined as an Actionforge graph in [`.github/workflows/graphs/build.act`](.github/workflows/graphs/build.act):

```
checkout -> run (node index.js)
```

It runs on every push to `main`, on pull requests, and on manual dispatch.
