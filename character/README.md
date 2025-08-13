# Character Query by ID

This project contains GraphQL queries to retrieve character details by ID using the `character(id: ID!)` field.

## Endpoint
https://rickandmortyapi.com/graphql

## Fields Requested
- id
- name
- status
- species
- type
- gender

## How to Run
1. Open a terminal.
2. Run:
```bash
curl -X POST \
  -H "Content-Type: application/json" \
  --data '{"query":"query { character(id: 1) { id name status species type gender } }"}' \
  https://rickandmortyapi.com/graphql | jq '.'
