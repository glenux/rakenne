# Entity-Relationship Diagrams - Domain Specific Language

## Goals

## Example

### An entity User

```
CREATE ENTITY User (
    id UUID,
    password_hash VARCHAR(250),
    role VARCHAR(10),
    created_at DATETIME,
    updated_at DATETIME
);
```

### An entity Url

```
CREATE ENTITY Url (
    id VARCHAR(250),
    custom_id VARCHAR(250),
    source_url TEXT,
    short_url VARCHAR(250),
    created_at DATETIME,
    updated_at DATETIME,
    expires_at DATETIME
);
```

### An relationship ManageLinks

```
CREATE RELATIONSHIP ManagesLinks (
  LINK User (0, N),
  LINK Url (
  HAS_ONE User,
  HAS_MANY Url,
  
  <attr> <attr_type>,
  <attr> <attr_type>,
  <attr> <attr_type>,
  <attr> <attr_type>,
);
```

