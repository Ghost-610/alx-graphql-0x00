# character

This directory contains GraphQL queries to fetch character details from the Rick and Morty GraphQL API using the `character(id: ID!)` field.

## Available Files

- `character-id-1.graphql` & `character-id-1-output.json`
- `character-id-2.graphql` & `character-id-2-output.json`
- `character-id-3.graphql` & `character-id-3-output.json`
- `character-id-4.graphql` & `character-id-4-output.json`

## How to Run a Query

Use `curl` to execute a `.graphql` file. For example:

```bash
curl -X POST https://rickandmortyapi.com/graphql \
  -H "Content-Type: application/json" \
  --data '{ "query": "{ character(id: 1) { id name status species type gender } }" }'
