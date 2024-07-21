# Food-Ordering-system-
A food ordering system using OOPS concepts of JAVA
Scope of the project (Functionalities included) – Food ordering system.
- Number of classes and its details along with relationships –
1. FoodItem:
 - Attributes
 - `name` (String): Represents the name of the food item.
 - `price` (double): Represents the price of the food item.
 - Methods:
 - `getName()`: Returns the name of the food item.
 - `getPrice()`: Returns the price of the food item.
 - `toString()`: Overrides the `toString` method to provide a string representation of 
the food item.
2. Order:
 - Attributes:
 - `items` (ArrayList<FoodItem>): Represents the list of food items in the order.
 - Methods:
 - `addItem(FoodItem item)`: Adds a food item to the order.
 - `getItems()`: Returns the list of food items in the order.
 - `calculateTotal()`: Calculates the total cost of the order by summing up the prices 
of all items.
3. FoodOrderingSystem:
 - Main class responsible for user interaction through the console.
 - Contains the `main` method where the execution starts.
 - Handles user input, creates instances of `FoodItem` and `Order`, and manages the 
order process.
Relationships:
- The `FoodItem` class is used to represent individual food items. Instances of 
`FoodItem` are created and added to the `Order`.
- The `Order` class manages a list of `FoodItem` objects, representing the items in the 
user's order.
- The `FoodOrderingSystem` class interacts with both `FoodItem` and `Order`. It 
creates instances of these classes, adds items to the order, and calculates the total cost.
Overall, there is a composition relationship between `Order` and `FoodItem`, as an 
`Order` "has a" list of `FoodItem` objects. The `FoodOrderingSystem` class interacts 
with both `FoodItem` and `Order`, coordinating the overall functionality of the food 
ordering system.
1. FoodItem Class:
 - Attributes:
 - `name` (String): Represents the name of the food item.
 - `price` (double): Represents the price of the food item.
 - Methods:
 - `getName()`: Returns the name of the food item.
 - `getPrice()`: Returns the price of the food item.
 - `toString()`: Provides a string representation of the food item.
2. Order Class:
 - Attributes:
 - `items` (ArrayList<FoodItem>): Represents the list of food items in the order.
 - Methods:
 - `addItem(FoodItem item)`: Adds a food item to the order.
 - `getItems()`: Returns the list of food items in the order.
 - `calculateTotal()`: Calculates the total cost of the order.
3. FoodOrderingSystem Class:
 - Manages user interaction through the console.
 - Creates instances of `FoodItem` and `Order`.
 - Handles ordering process based on user input.
These classes work together to create a basic Food Ordering System with food items, 
orders, and a simple console interface.
- Use of packages
1. model Package:
 - `FoodItem` class: Represents a food item.
 - `Order` class: Represents an order.
java
package model;
public class FoodItem { /* ... */ }
java
package model;
import java.util.ArrayList;
public class Order { /* ... */ }
2. system Package:
 - `FoodOrderingSystem` class: Manages user interactions and the ordering process.
java
package system;
import model.FoodItem;
import model.Order;
import java.util.ArrayList;
public class FoodOrderingSystem { /* ... */ }
