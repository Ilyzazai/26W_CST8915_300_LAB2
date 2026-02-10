# Lab 2 – CST8915

## Youtube Video


---

## Service Repositories

- **Order Service (Node.js)**  
  https://github.com/Ilyzazai/order-service
  
- **Product Service (Rust)**  
  https://github.com/Ilyzazai/product-service

- **Store Front (Vue.js)**  
  https://github.com/Ilyzazai/store-front
---



### 1. What changes did you make to comply with Config and Backing Services?
The services were refactored to remove hard-coded configuration . Environment variables were created using `.env` files during development to configure ports and service connection URLs. RabbitMQ was treated as an external backing service by configuring its connection s through environment variables instead of connecting it in the code.

### 2. Why use environment variables instead of hard-coded values?
Environment variables allow the same code to be deployed in different environments without changes. it improves security, flexibility, and portability, and aligns with cloud-native best practices.

### 3. Why separate repositories for each microservice?
Each microservice has its own lifecycle, dependencies, and deployment process. Separate repositories improve maintainability, scalability, and allow teams to work independently on different services.

---

## Notes
Some components were tested locally due to time and resource constraints.
