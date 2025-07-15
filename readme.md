# Local Router

## Overview

This project is a local router implementation that allows for running apollo gql federation services locally.

## Usage

first add subgrpah schema to subgraph folder

update supergraph.yaml accordingly

compose supergraph schema with the command, rover cli should be installed - https://www.apollographql.com/docs/rover/getting-started:

```bash
rover supergraph compose --config ./supergraph.yaml --output ./supergraph.graphql --log info
```

start local router with the command:

```bash
./router --dev --config router.yaml --supergraph supergraph.graphql
```
