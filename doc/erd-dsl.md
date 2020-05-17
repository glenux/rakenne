# Entity-Relationship Diagrams - Domain Specific Language

## Goals

* Describe all possible cases according to MERISE
* Be simple to read and write by a human user
* Be simple to parse by a machine

## Example

```
entities:
  user:
    - name: id
      type: uuid
      key: true
    - name: password_hash
      type: varchar
      limit: 250
    - name: role
      type: varchar
      limit: 10
    - name: created_at
      type: datetime
    - name: updated_at
      type: datetime
  url:
    - name: id
      type: varchar
      limit: 250
      key: true
    - name: custom_id
      type: varchar
      limit: 250
    - name: source_url
      type: text
    - name: short_url
      type: varchar
      limit: 250
    - name: created_at
      type: datetime
    - name: updated_at
      type: datetime
    - name: expires_at
      type: datetime

relationships:
  manages_urls:
    links:
      - name: user: 
        equals: 1
      - name: url:
        min: 0
        max: n
    properties: []
```
