# Santader BootCamp 
Java RESTFul API criada para o SantaderBootCamp

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        +String name
        +Account account
        +List~Feature~ features
        +Card card
        +List~News~ news
    }

    class Account {
        +String number
        +String agency
        +String balance
        +String limit
    }

    class Feature {
        +String icon
        +String description
    }

    class Card {
        +String number
        +String limit
    }

    class News {
        +String icon
        +String description
    }

    User "1" *--"1" Account
    User "1" *--"N" Card
    User "1" *--"1" Feature
    User "1" *--"N" News
```
