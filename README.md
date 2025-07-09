# 🛒 OSOM E-Commerce Clone – Full-Stack E-commerce Web Application

A production-style e-commerce platform replicating the user experience of OSOM, built with modern technologies and secure integrations.

[🌐 Live Demo](https://osom-in-clone-frontend.vercel.app/)

---

## 🚀 Features

- 🛍️ **Product Catalog**  
  Browse products with dynamic filtering and search.

- 👤 **User Accounts**  
  Secure registration, login, and order management.

- 🛒 **Shopping Cart & Checkout**  
  Add items to the cart, review orders, and complete purchases.

- 💳 **Stripe Payments**  
  Seamless and secure payment processing.

- 🖼️ **Image Hosting via Cloudinary**  
  Efficient storage and delivery of product images.

- 🗄️ **Database:**  
  Uses **MySQL** (managed via Aiven) for robust, cloud-based data storage.

---

## 🛠️ Tech Stack

- **Frontend:** Next.js and bootstrap for server-side rendering and responsive UI
- **Backend:** Java & Spring Boot providing RESTful APIs
- **Database:** MySQL (Aiven-managed) for cloud-based data storage
- **Image Hosting:** Cloudinary
- **Payments:** Stripe API

---

## 📂 Repositories

| Part       | Repository Link |
|------------|-----------------|
| 🌐 Frontend | [Frontend Repository](https://github.com/megha0705/Osom.in_clone_frontend) |
| 🛠️ Backend | [Backend Repository](https://github.com/megha0705/osom.in-clone-backend) |


---
## ⚙️ Running Locally

To set up the application locally, you need to run **both** frontend and backend services.

---

📥 Clone the Repository


git clone https://github.com/megha0705/Osom.in.Clone


cd osom.in_clone

🔧 Backend Setup


1. Add Dependencies to pom.xml
xml   
<!-- Cloudinary for image management -->
<dependency>
    <groupId>com.cloudinary</groupId>
    <artifactId>cloudinary-http44</artifactId>
    <version>1.33.0</version>
</dependency>

<!-- Stripe for payments -->
<dependency>
    <groupId>com.stripe</groupId>
    <artifactId>stripe-java</artifactId>
    <version>24.7.0</version>  
</dependency>

<!-- MySQL Connector -->
<dependency>
    <groupId>com.mysql</groupId>
    <artifactId>mysql-connector-j</artifactId>
    <scope>runtime</scope>
</dependency>

2. Configure application.properties
   
properties
# Database Configuration
spring.datasource.url=jdbc:mysql://<your-mysql-url>/<database>
spring.datasource.username=<username>
spring.datasource.password=<password>

# Cloudinary Configuration
cloudinary.api-key=<your-api-key>
cloudinary.cloud-name=<your-cloud-name>
cloudinary.api-secret=<your-secret-key>

# Stripe Configuration
stripe.webhook.secret=<your-stripe-secret-key>
3. Build and Run the Spring Boot Server
Option 1: Run directly from IDE

Navigate to src/main/java/com/Osom/demo/

Run OsomApplication.java

Option 2: Use Maven commands


./mvnw clean install
./mvnw spring-boot:run

💻 Frontend Setup

cd frontend
npm install       # Install dependencies
npm run dev      # Start development server

The application will be available at:
👉 http://localhost:3000

🔑 Required Services
Make sure you have accounts and API keys for:

MySQL Database

Cloudinary (for image storage)

Stripe (for payments)







