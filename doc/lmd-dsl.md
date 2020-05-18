## Logical Model - DSL

```yaml
tables:
  user:
    name: "Utilisateur"
    properties:
      - name: id
        type: integer
        key: true
        options: ['autoincrement']
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
    name: "Adresses"
    properties:
      - name: id
        type: varchar
        limit: 250
        key: true
      - name: user
        type: reference
        table: user
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

constraints:
  # do we need constraints here?
```
