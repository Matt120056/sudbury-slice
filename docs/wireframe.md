# Sudbury Slice: Main Screen Wireframe

## Main Screen Layout

+--------------------------------------------------+
| [1]              S U D B U R Y  S L I C E       |
|                                      [Profile]   |
+--------------------------------------------------+
| [2]              WELCOME TO SUDURY SLICE         |
|          Find your next favourite pizza!         |
+--------------------------------------------------+
| [3]                 SEARCH PIZZAS                |
|       [ Search by pizza name...          ]       |
+--------------------------------------------------+
| [4]                 PIZZA MENU                   |
|                                                  |
|  +----------------------+  +------------------+  |
|  |      [Pizza Image]   |  |   [Pizza Image]  |  |
|  |   Pineapple Pizza    |  |  Cheese Pizza    |  |
|  |       $15.99         |  |     $18.99       |  |
|  |      Rating: 5.0     |  |    Rating: 4.3   |  |
|  |      [View Pizza]    |  |   [View Pizza]   |  |
|  +----------------------+  +------------------+  |
|                                                  |
+--------------------------------------------------+
| [5]              POPULAR TOPPINGS                |
|                                                  |
|       Pepperoni | Mushrooms | Olives | Peppers   |
|                                                  |
+--------------------------------------------------+
| [6]                 BOTTOM NAVIGATION            |
|                                                  |
|       [Home]       [Pizzas]       [My Profile]   |
+--------------------------------------------------+


## Legend

1. **App Header:** Displays the Sudbury Slice name and profile button. Reads `tblCustomer` to retrieve the logged-in customer's profile information.

2. **Welcome Section:** Displays a welcome message to the customer. No database table required.

3. **Search Bar:** Allows customers to search for pizzas by name. Reads `tblPizza` to find matching pizzas.

4. **Pizza Menu:** Displays available pizzas, prices, images, and average customer ratings. Reads `tblPizza` for pizza information and `tblRating` for customer ratings.

5. **Popular Toppings:** Displays available toppings customers can add to their pizzas. Reads `tblTopping` for topping names and details.

6. **Bottom Navigation:** Allows customers to navigate between Home, Pizzas, and My Profile. Reads `tblCustomer` when loading the customer's profile.
