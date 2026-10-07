# 🛠 Workshop: Tactical Domain-Driven Design

Welcome to the practical workshop on Domain-Driven Design! 
The goal of this session is to translate the theoretical concepts from the book *Learning Domain-Driven Design* into real, working code.

We intentionally **do not provide a predefined folder structure or architectural scaffolding**. Designing the project layout is entirely up to you and is part of the challenge! 

You are highly encouraged to experiment with and apply any pattern you deem appropriate from the book, including:
*   **Hexagonal Architecture (Ports and Adapters)**
*   **Aggregate Roots, Entities, and Value Objects**
*   **Application Services and Domain Services**
*   **Domain Events**

You can start by modeling a "pure" domain driven by Unit Tests, and then wire up your favorite ORMs, Web Frameworks, and Databases to see how your domain integrates with infrastructure.

## 🚀 How to Participate

1. **Fork** this repository to your GitHub account.
2. Clone your fork locally: `git clone https://github.com/YOUR-ACCOUNT/ddd-tactical-kata.git`
3. Create a branch with your name: `git checkout -b kata-name-surname`
4. Choose one of the three folders (01, 02, or 03) and explore the requirements in its `README.md`.
5. Open a **Draft Pull Request** immediately against the original repository. This allows the facilitator and other participants to see your progress, discuss architectural choices, and provide real-time feedback.
6. Design your architecture, write your tests, and have fun!

## 📂 The Projects (Choose ONE)

* **[01 - Shopping Cart](./01-Shopping-Cart/) (Level: Basic)**: Learn to protect simple invariants and use the power of Value Objects to handle currencies safely.
* **[02 - Coworking Desks](./02-Coworking-Desks/) (Level: Intermediate)**: Deal with time, state transitions, and identity. Create robust logic to prevent overlapping schedules.
* **[03 - Hazmat Logistics](./03-Hazmat-Logistics/) (Level: Advanced)**: Manage complex Aggregate Roots that must coordinate child entities with conflicting and strict chemical rules.
