# Entity-Relationship Diagrams - Domain Specific Language

## Goals

## Example

### An entity User

```
ENTITY User {
    id: UUID,
    password_hash: VARCHAR(250),
    role: VARCHAR(10),
    created_at: DATETIME,
    updated_at: DATETIME
}
```

### An entity Url

```
ENTITY Url {
    id: VARCHAR(250),
    custom_id: VARCHAR(250),
    source_url: TEXT,
    short_url: VARCHAR(250),
    created_at: DATETIME,
    updated_at: DATETIME,
    expires_at: DATETIME
};
```

### An relationship ManageLinks

```
RELATIONSHIP ManagesLinks {
  LINK User (1, 1),
  LINK Url (0, N),
};
```
