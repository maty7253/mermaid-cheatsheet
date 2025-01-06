# Entity Relationship Diagrams

ER diagrams show the relationships between entities in a database.

## Basic Syntax

```mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ LINE-ITEM : contains
    CUSTOMER }|..|{ DELIVERY-ADDRESS : uses
```

## Relationship Types

```mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : "one-to-many"
    STUDENT }|--|{ CLASS : "many-to-many"
    DRIVER ||--|| CAR : "one-to-one"
```

## Attributes

```mermaid
erDiagram
    CAR {
        string registrationNumber PK
        string make
        string model
        string[] parts
    }
    DRIVER {
        string licenseNumber PK
        string name
        integer age
    }
```

## Cardinality and Key Types

- `|o` - Zero or one
- `||` - Exactly one
- `}o` - Zero or many
- `}|` - One or many

