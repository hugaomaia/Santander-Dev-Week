# Santander Dev Week
Java RESTful API criada para a Santander Dev Week.

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        +String name
        +Account account
        +Feature[] features
        +Card card
        +News[] news
    }
    class Account {
        +String number
        +String agency
        +Number balance
        +Number limit
    }
    class Feature {
        +String icon
        +String description
    }
    class Card {
        +String number
        +Number limit
    }
    class News {
        +String icon
        +String description
    }
    User "1"*-- "1" Account : contains
    User "1"*-- "N" Feature : contains
    User "1"*-- "1" Card : contains
    User "1"*-- "N" News : contains
```
