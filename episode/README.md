# Episode Query by ID

This project contains a GraphQL query to retrieve details of a specific episode using the `episode(id: ID!)` field.

## Endpoint
https://rickandmortyapi.com/graphql

## Fields Requested
- id
- name
- air_date
- episode

## How to Run
Example for episode with ID 1:
```bash
curl -X POST \
  -H "Content-Type: application/json" \
  --data '{"query":"query { episode(id: 1) { id name air_date episode } }"}' \
  https://rickandmortyapi.com/graphql | jq '.'
