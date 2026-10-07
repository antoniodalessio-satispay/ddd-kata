# 🛒 Kata 01: The E-commerce Shopping Cart

## Business Context
We are upgrading our e-commerce platform to support global sales. In the past, the system had critical bugs because it mixed up different currencies and miscalculated promotional discounts. Your task is to implement the core shopping cart engine, ensuring that all business rules are strictly enforced at all times.

## Business Requirements

1. **Capacity Limit:** A shopping cart cannot contain more than 50 physical items in total.
2. **Currency Consistency:** A cart can only process a single currency at a time. The first item added to an empty cart establishes the cart's currency. Any subsequent attempt to add a product with a different currency (e.g., trying to add a $10 item to a cart already containing a €15 item) must be rejected by the system.
3. **Shipping Costs:** Standard shipping costs 5.00 in the cart's currency. However, if the subtotal of the items in the cart exceeds 100.00, the shipping cost is automatically waived (becomes 0.00).
4. **Discount Codes:** 
   - A customer can apply a maximum of one discount code per cart. 
   - The code `"MINUS20"` reduces the total item cost by 20%.
   - **Exception:** The 20% discount does **not** apply to products that are explicitly flagged as "On Sale". Those items retain their original price, while the rest of the eligible items get the discount.

## Technical Scope
This is a greenfield project. You are building this application from scratch. You are completely free to set up the project using any web framework (Spring Boot, ASP.NET Core, Express, etc.), any ORM, and any database of your choice, or you can keep the persistence entirely in-memory. The goal is to demonstrate how your Domain Model guarantees the business rules and how you choose to connect it to the infrastructure and API layers.
