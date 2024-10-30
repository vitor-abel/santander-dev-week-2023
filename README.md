#Santander Dev Week 2023
Java RESTful API criada para a Santander Dev Week.

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        -String name
        -Account account
        -Card card
        -Feature[] features
        -News[] news
    }

    class Account {
        -String number
        -String agency
        -Number balance
        -Number limit
    }

    class Card {
        -String number
        -Number limit
    }

    class Feature {
        -String icon
        -String description
    }

    class News {
        -String icon
        -String description
    }

    User --> Account
    User --> Card
    User --> Feature
    User --> News
