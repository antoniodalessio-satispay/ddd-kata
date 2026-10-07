# 🏢 Kata 02: Coworking Desk Booking

## Business Context
We run a premium coworking space. Desks are our most valuable resource. We need a booking system that ensures maximum occupancy without ever double-booking a desk, while also handling inevitable maintenance issues smoothly.

## Business Requirements

1. **Standardized Time Blocks:** Customers cannot book desks for arbitrary hours. Bookings are strictly limited to three available time slots:
   - Morning Half-Day: 08:00 to 13:00
   - Afternoon Half-Day: 14:00 to 19:00
   - Full-Day: 08:00 to 19:00
2. **Zero Overbooking:** A desk can never be booked by more than one person for the same time slot (e.g., a Morning booking conflicts with a Full-Day booking for the same desk on the same day).
3. **Out of Service / Maintenance:** Desks sometimes break (e.g., broken monitors or spilled coffee). A desk can be marked as "Out of Service". The moment this happens, all future bookings associated with that specific desk must be immediately canceled, and the system must flag them for a full refund.
4. **Cancellation Policy:** 
   - Customers can cancel their bookings. 
   - If a cancellation occurs more than 24 hours before the booking's start time, the customer receives a 100% refund. 
   - If the cancellation occurs less than 24 hours before the start time, the customer receives only a 50% refund.

## Technical Scope
This is a greenfield project. You are building this application from scratch. You are completely free to set up the project using any web framework (Spring Boot, ASP.NET Core, Express, etc.), any ORM, and any database of your choice, or you can keep the persistence entirely in-memory. The goal is to demonstrate how your Domain Model guarantees the business rules and how you choose to connect it to the infrastructure and API layers.
