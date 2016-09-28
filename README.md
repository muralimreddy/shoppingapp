__Shopping App Using Spring Microservices Concepts__

This project will use following Spring Microservice concepts
- 1. Spring Cloud 
- 2. Eureka Server
- 3. Netflix Feign (Ribbon)
- 4. Config Server
- 5. Netflix Zuul

Database: H2

Product Service
This service will provide product details like
1. Title of product
2. SKU
3. Price

Product service will be running in three instances:
Ports: 8021, 8022, 8023

Product Inventory Service:
This service will provide the inventory details. It will take SKU as input and provides quantity of the item. 
This service will run in three instances on ports: 8026, 8027, 8028

Product Catalog Service:

This service will consume Product service and Inventory service and provide a catalog to the UI
This service will also run in three instances on ports: 8031, 8032,8033


