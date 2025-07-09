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

To set up the application locally, you need to run both frontend and backend services.

### 1️⃣ Clone the repository

git clone https://github.com/megha0705/Osom.in.Clone
cd osom.in_clone

### 2️⃣ Set up and run the backend
**Add dependency in pom.xml file**

	<dependency>
			<groupId>com.cloudinary</groupId>
			<artifactId>cloudinary-http44</artifactId>
			<version>1.33.0</version>
		</dependency>


		<dependency>
			<groupId>com.stripe</groupId>
			<artifactId>stripe-java</artifactId>
			<version>24.7.0</version>  
		</dependency>


  <dependency>
			<groupId>com.mysql</groupId>
			<artifactId>mysql-connector-j</artifactId>
			<scope>runtime</scope>
		</dependency>
<!-- Check for the latest version -->

**Configure your application.properties with your MySQL connection details and API keys**

spring.datasource.url=jdbc:mysql://<your-mysql-url>/<database>
spring.datasource.username=<username>
spring.datasource.password=<password>

cloudinary.api-key =<yourapikey>
cloudinary.cloud-name = <yourcloudname>
cloudinary.api-secret = <yoursecretkey>

stripe.webhook.secret = <stripespikey>

**Build and run springboot server**

cd src/main/java/com/Osom/demo/
Run OsomApplication.java file
**Or**
./mvnw clean install
./mvnw spring-boot:run

## 3️⃣ Install and run the Frontend

cd ../frontend

**Install dependencies**

npm install

**Start the development server**

npm run dev
Visit http://localhost:3000 in your browser.







