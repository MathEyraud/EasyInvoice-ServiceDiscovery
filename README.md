# Project EasyInvoice
## EasyInvoice Service Discovery (service-discovery)
### Description:
The service-discovery module uses Spring Cloud Netflix Eureka for service registration and discovery. It ensures that all microservices (customer, invoice, product) can dynamically discover each other and communicate effectively.

### Key Features:
- Service registration and discovery using Eureka.
- Centralized configuration for microservices communication.

## Integration Overview
EasyInvoice is designed as a microservices architecture where each service has a distinct responsibility. The invoice-core module provides the shared entity definitions, while the customer, invoice, and product services handle their respective domains. The service-discovery module facilitates dynamic discovery and communication among these services.
- Customer Service: Provides customer data to the Invoice service. https://github.com/MathEyraud/EasyInvoice-Customer
- Invoice Service: Manages invoices and retrieves necessary customer and product data from respective services. https://github.com/MathEyraud/EasyInvoice-Invoice
- Product Service: Supplies product information to the Invoice service. https://github.com/MathEyraud/EasyInvoice-Product
- Service Discovery: Ensures all services can discover and communicate with each other. https://github.com/MathEyraud/EasyInvoice-ServiceDiscovery
- Invoice Core: https://github.com/MathEyraud/Java-Learn-Spring-Data-Core/tree/Microservices
This architecture ensures scalability, modularity, and ease of maintenance, making EasyInvoice a robust and flexible invoicing solution.
