# Santander Dev
Java RESTful API criada para  aplicação Santander.

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        +string name
        +Account account
        +Card card
        +Feature[] features
        +News[] news
    }

    class Account {
        +string number
        +string agency
        +float balance
        +float limit
    }

    class Card {
        +string number
        +float limit
    }

    class Feature {
        +string icon
        +string description
    }

    class News {
        +string icon
        +string description
    }

    User *-- Account
    User *-- Card
    User *-- Feature
    User *-- News
```
