# SliceDB: Entity-Relationship Diagram
**Designed by:** Matt Pheaton

mermaid
erDiagram
    tblCustomer {
        int CID PK
        string FirstName
        string LastName
        string Email
        string City
        date DateJoined
    }
    tblPizza {
        int PID PK
        string PizzaName
        string Category
        decimal BasePrice
    }
    tblTopping {
        int TID PK
        string ToppingName
        string Vegan
        decimal ExtraCost
    }
    tblCustomer ||--o{ tblRating : writes

## My design decisions
One pizza has many toppings and one topping is on many pizzas, and a database can’t store that many-to-many link in either table alone.
A separate table holds one row for each “this topping is on this pizza” fact. 
 
PTID gives every pizza-topping row its own unique identifier, so each row can be found, changed or deleted by itself without relying on a combination of PID and TID.

Leaving a written comment is optional. A customer can give just a star rating, so the Remark column has to be allowed to stay empty. 
 
Note: tblPizzaTopping exists because people need their toppings 
