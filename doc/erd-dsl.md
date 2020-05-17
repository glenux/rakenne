# Entity-Relationship Diagrams - Domain Specific Language

## Goals

## Example

```
entities:
  user:
    id: UUID
    password_hash: VARCHAR(250)
    role: VARCHAR(10)
    created_at: DATETIME
    updated_at: DATETIME
  url:
    id: VARCHAR(250)
    custom_id: VARCHAR(250)
    source_url: TEXT
    short_url: VARCHAR(250)
    created_at: DATETIME
    updated_at: DATETIME
    expires_at: DATETIME

relationships:
  manages_urls:
    links:
      - user: 
          eq: 1
      - url
          gte: 0
          lte: n
    properties: {}
```
