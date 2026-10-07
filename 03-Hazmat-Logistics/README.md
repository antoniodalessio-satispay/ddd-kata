# ☢️ Kata 03: Hazardous Materials (Hazmat) Logistics

## Business Context
You are building the stowage validation system for sea freight containers carrying hazardous materials (Hazmat). Safety regulations are incredibly strict: a single rule violation during the loading process risks severe fines or catastrophic accidents at sea. 

## Business Requirements

1. **Maximum Weight Capacity:** Every shipping container is manufactured with a specific maximum payload capacity (e.g., 1000 kg). The total weight of all loaded barrels can never exceed this limit.
2. **Chemical Segregation:** Materials categorized as `Explosive` and `Flammable` are strictly incompatible. Under no circumstances can an explosive barrel and a flammable barrel be loaded into the same container.
3. **Toxic Material Protocol:** Materials categorized as `Toxic` require a significant spatial safety buffer. Whenever a toxic barrel is loaded into a container, it instantly reduces the container's *remaining available capacity* by an additional 10% (calculated on the toxic barrel's weight). 
   *Example: A container has 500 kg of capacity remaining. You load a 100 kg toxic barrel. The standard remaining capacity drops to 400 kg, but due to the 10% toxic penalty (10 kg), the actual remaining capacity drops to 390 kg.*
4. **Traceability:** No barrel can be loaded onto a container unless it has a clearly defined, non-empty batch number registered in the system.

## Technical Scope
This is a greenfield project. You are building this application from scratch. You are completely free to set up the project using any web framework (Spring Boot, ASP.NET Core, Express, etc.), any ORM, and any database of your choice, or you can keep the persistence entirely in-memory. The goal is to demonstrate how your Domain Model guarantees the business rules and how you choose to connect it to the infrastructure and API layers.
