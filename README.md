# Design Patterns in Java

This project showcases the implementation of ten different design patterns in Java. Each pattern is organized into its own package, with the primary classes and interfaces separated into individual files for better modularity and readability.

## Implemented Design Patterns:
1. **Strategy Pattern**: A dynamic payment system that can handle different payment methods (e.g., Credit Card, PayPal, Cryptocurrency).
   - **Package**: `StrategyPattern`
   - **Classes**: `PaymentStrategy`, `CreditCardPayment`, `PayPalPayment`, `CryptoPayment`, `ShoppingCart`

2. **Observer Pattern**: A weather tracking system that updates various display units when there are changes in the weather data.
   - **Package**: `ObserverPattern`
   - **Classes**: `Observer`, `WeatherStation`, `CurrentConditionsDisplay`

3. **Command Pattern**: A smart remote control system for controlling various devices (e.g., lights) by issuing commands.
   - **Package**: `CommandPattern`
   - **Classes**: `Command`, `Light`, `LightOnCommand`, `RemoteControl`

4. **State Pattern**: An order management system where the order transitions through various states (e.g., New, Paid, Shipped).
   - **Package**: `StatePattern`
   - **Classes**: `OrderState`, `NewOrder`, `PaidOrder`, `ShippedOrder`, `DeliveredOrder`, `Order`

5. **Chain of Responsibility Pattern**: An expense approval system where requests are processed by a series of approvers (e.g., Team Lead, Manager, Director).
   - **Package**: `ChainOfResponsibilityPattern`
   - **Classes**: `Approver`, `TeamLead`, `Manager`, `Director`

6. **Mediator Pattern**: A chat system where users communicate with each other through a mediator.
   - **Package**: `MediatorPattern`
   - **Classes**: `ChatMediator`, `ChatRoom`, `User`, `RegularUser`

7. **Memento Pattern**: A system for document version control, allowing users to save and retrieve previous versions of a document.
   - **Package**: `MementoPattern`
   - **Classes**: `Document`, `DocumentMemento`, `VersionControl`

8. **Visitor Pattern**: A system to calculate the area of different shapes using the visitor pattern.
   - **Package**: `VisitorPattern`
   - **Classes**: `Shape`, `Circle`, `Rectangle`, `Visitor`, `AreaCalculator`

9. **Template Method Pattern**: A report generation system that allows different formats (e.g., PDF, HTML) to be created using a common template structure.
   - **Package**: `TemplateMethodPattern`
   - **Classes**: `ReportGenerator`, `PDFReportGenerator`

10. **Iterator Pattern**: A playlist system that supports traversal of songs using different types of iterators.
   - **Package**: `IteratorPattern`
   - **Classes**: `Playlist`, `Song`

## How to Execute:
- Each design pattern has a demonstration in the `Main.java` file, located in the root directory.
- To run the examples, compile and execute the `Main.java` file, which demonstrates all 10 design patterns.

## Project Structure:
- Each design pattern is encapsulated within its respective package.
- The associated classes and interfaces are placed in separate files for clarity and modular design.
- Example code demonstrating the usage of each design pattern is included in `Main.java`.

## Example Code:
```java
public class Main {
    public static void main(String[] args) {
        // Strategy Pattern Example
        ShoppingCart cart = new ShoppingCart();
        cart.setPaymentStrategy(new CreditCardPayment());
        cart.checkout(100);

        // Further examples for other patterns...
    }
}
```

## System Requirements:
- JDK version 8 or higher is required to run this project.


