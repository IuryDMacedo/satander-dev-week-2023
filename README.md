# Satander Dev Week 2023

### Projeto final do BootCamp DIO com Santander.
criação de uma pequena conta bancaria do aplicativo do santander.

## Diagrama de Classes 

```mermaid
classDiagram
  class User {
    - name: String
    -Account: account
    -Feature[] features
    -Card card
    -News[] news
  }

  class Account {
    - number: String
    - agency: String
    - balance: double
    - limit: double
  }

  class Feature {
    - icon: String
    - description: String
  }

  class Card {
    - number: String
    - limit: double
  }

  class News {
    - icon: String
    - description: String
  }

  User "1"  *-- "1" Account
  User "1"  *-- "N" Feature
  User "1" *-- "N" News
  User "1" *-- "1" Card
```
