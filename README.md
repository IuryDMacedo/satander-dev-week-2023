# Satander Dev Week 2023
Java RESTful API criada para a santander Dev Week

## Diagrama de Classes 

```mermaid
classDiagram
  class User {
    - name: String
    + getBalance(): double
    + getLimit(): double
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
