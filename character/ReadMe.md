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


# Characters Pagination Queries

This directory contains GraphQL queries to fetch a paginated list of characters from the API.

- **characters-page-1.graphql** → Query for page 1
- **characters-page-1-output.json** → Response for page 1
- **characters-page-2.graphql** → Query for page 2
- **characters-page-2-output.json** → Response for page 2
- **characters-page-3.graphql** → Query for page 3
- **characters-page-3-output.json** → Response for page 3
- **characters-page-4.graphql** → Query for page 4
- **characters-page-4-output.json** → Response for page 4

Each query fetches the following fields:
- `id`
- `name`
- `status`
- `image`

```

# Episode Query

This directory contains GraphQL queries to fetch details of an episode from the Rick and Morty GraphQL API.

- **episode-page-1.graphql** → Query for episode with id 1
- **episode-page-1-output.json** → Response for episode with id 1

Each query fetches:
- `id`
- `name`
- `air_date`
- `episode`
