# 26W_CST8915_300_LAB2

# Lab 2 – CST8915: 12-Factor App Refactor

## Demo Video
YouTube (Unlisted):  
👉 PASTE YOUR YOUTUBE LINK HERE

---

## Service Repositories

- **Order Service (Node.js)**  
  https://github.com/YOUR_USERNAME/order-service

- **Product Service (Rust)**  
 

- **Store Front (Vue.js)**  

---

## Reflection

### 1. What changes did you make to comply with Config and Backing Services?
The services were refactored to remove hard-coded configuration values. Environment variables were introduced using `.env` files during development to configure ports and service connection URLs. RabbitMQ was treated as an external backing service by configuring its connection string through environment variables instead of embedding it in the code.

### 2. Why use environment variables instead of hard-coded values?
Environment variables allow the same codebase to be deployed in different environments without modification. This improves security, flexibility, and portability, and aligns with cloud-native best practices.

### 3. Why separate repositories for each microservice?
Each microservice has its own lifecycle, dependencies, and deployment process. Separate repositories improve maintainability, scalability, and allow teams to work independently on different services.

---

## Notes
Some components were tested locally due to time and resource constraints. The configuration supports deployment across separate VMs as required.
