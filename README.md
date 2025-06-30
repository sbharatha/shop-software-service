The Jewellery Shop Management System is a full-stack application designed to streamline operations for retail jewellery businesses. Built with Spring Boot, PostgreSQL, and React (frontend pending), the system efficiently manages gold and silver product inventory, including product creation, updates, categorization, and validation of business rules.

Core Features:

✅ Product Management: Add, view, update, and delete jewellery products (gold/silver), including attributes like weight, purity, making charges, and removable items (stones, pearls, etc.).

🏷️ Barcode & ID Generation: Automatically generate unique product IDs and barcodes using UUIDs for traceability.

⚖️ Weight & Cost Calculations: Automatically calculate net weight, total cost, and VA (Value Addition) weight using configurable logic.

🔒 Business Rule Validation: Enforce jewellery-specific rules (e.g., gold items must have VA type and purity; net weight must not exceed gross weight).

📊 Inventory Views: Fetch all products, gold-only, silver-only, or filter by stock availability (available, sale return, defect).

⚠️ Error Handling & Logging: Structured logging and custom error codes for meaningful backend exceptions.

🔁 Update Flow with Removable Items: Safe update logic that retains and updates individual removable stones with validation.

Technologies Used:

Backend: Java 21, Spring Boot 3.5.x, Spring Data JPA

Database: PostgreSQL

Validation: Jakarta Bean Validation (e.g., @DecimalMin, @NotNull)

Logging: SLF4J with structured log messages

Error Management: Custom error codes and ResponseStatusException for HTTP status responses

(Frontend planned using React + Tailwind)

Ideal For:

Jewellery shops managing physical inventory

Digitizing sales, returns, and item tracking

Businesses needing fine-grained control over items with embedded stones or removable parts
