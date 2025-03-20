# 👤 **User Service API – Scalable & Secure User Management** 🚀  

![.NET 10](https://img.shields.io/badge/.NET%2010-blue?style=for-the-badge)  
![MongoDB](https://img.shields.io/badge/MongoDB-%E2%9C%85-green?style=for-the-badge)  
![Microservices](https://img.shields.io/badge/Microservices-%F0%9F%92%BB-purple?style=for-the-badge)  
![Docker](https://img.shields.io/badge/Docker-%F0%9F%90%A6-blue?style=for-the-badge)  
![Secure API](https://img.shields.io/badge/Secure%20API-%F0%9F%94%92-red?style=for-the-badge)  

Welcome to **User Service API**, a **high-performance, containerized user management microservice** built with **.NET 10 and MongoDB**. Designed for **scalability and efficiency**, this API follows **Clean Architecture principles** and is optimized for **modern web applications and microservices**.  

> **Why Use User Service API?**  
> - 🚀 **Fast and Scalable** – Built with **NoSQL and optimized queries**  
> - 🔒 **Secure and Reliable** – Implements **best security practices**  
> - 🛠 **Docker-Ready** – Fully containerized with **Docker Compose support**  
> - 📡 **Modern & Maintainable** – Uses **Clean Architecture and Repository Pattern**  

---

## **🌟 Features**  

✅ **Full CRUD Operations** – Manage users with **RESTful API endpoints**  
✅ **MongoDB Integration** – NoSQL database for **scalability and performance**  
✅ **Containerized Deployment** – **Docker support** for seamless cloud deployment  
✅ **Clean Architecture** – **Separation of concerns** for maintainability  
✅ **OpenAPI Documentation** – Auto-generated API docs with **Swagger UI**  
✅ **Secure by Design** – **HTTPS enabled & authentication-ready**  
✅ **Optimized for Cloud & Microservices** – Works with **Kubernetes, AWS, and Azure**  

---

## **🏗️ Architecture & Design Patterns**  

📌 **Clean Architecture** – Separates concerns into:  
   - **Application Layer** – Business logic, validation, and MediatR commands.  
   - **Domain Layer** – Core **user models and validation rules**.  
   - **Persistence Layer** – Handles **MongoDB data access**.  
   - **Infrastructure Layer** – Logging, authentication, and notifications.  
   - **API Layer** – **Minimal API** for performance & simplicity.  

📌 **Repository Pattern** – Encapsulates data access for **MongoDB**.  
📌 **Dependency Injection** – Ensures modular and testable code.  
📌 **Docker-First Approach** – Easily deployable in **cloud-native environments**.  

---

## **📂 Project Structure**  

📌 **src/UserService.Api** – Main API layer with controllers and endpoints.  
📌 **src/UserService.Application** – Business logic and command handlers.  
📌 **src/UserService.Domain** – Core models and domain rules.  
📌 **src/UserService.Infrastructure** – MongoDB integration, logging, and security.  
📌 **tests/UserService.Tests** – Unit and integration test cases.  
📌 **docker-compose.yml** – Configurations for **API and MongoDB containers**.  

---

## **🚀 Getting Started**  

### **📌 Prerequisites**  
✅ [.NET 10 SDK](https://dotnet.microsoft.com/download)  
✅ [Docker](https://www.docker.com/products/docker-desktop)  
✅ [MongoDB](https://www.mongodb.com/)  

### **Step 1: Clone the Repository**  
```bash
git clone https://github.com/yourusername/UserServiceAPI.git
cd UserServiceAPI
```

### **Step 2: Run with Docker Compose**  
```bash
docker-compose up -d
```

The API will be available at:  
🔹 **HTTP:** `http://localhost:8080`  
🔹 **HTTPS:** `https://localhost:8081`  

---

## **🌍 API Endpoints**  

### **👥 User Management**  
| Method | Endpoint | Description |
|--------|---------|-------------|
| **GET**  | `/api/user` | Retrieves all users (with pagination) |
| **GET**  | `/api/user/{id}` | Fetches user details by ID |
| **POST** | `/api/user` | Creates a new user |
| **PUT**  | `/api/user/{id}` | Updates an existing user |
| **DELETE** | `/api/user/{id}` | Deletes a user |

### **📊 Health & Status**  
| Method | Endpoint | Description |
|--------|---------|-------------|
| **GET**  | `/health` | Checks API and database health |

### **Example Request (cURL)**  
```bash
curl -X POST http://localhost:8080/api/user \
  -H "Content-Type: application/json" \
  -d '{
    "name": "John Doe",
    "username": "johndoe",
    "email": "john@example.com",
    "phoneNumber": "+15551234567"
  }'
```

---

## **🔧 Configuration**  

Modify `appsettings.json` to update database settings:  

```json
{
  "ConnectionStrings": {
    "MongoDb": "mongodb://admin:Test123!@mongo:27017"
  },
  "DatabaseName": "UserDB"
}
```

---

## **🧪 Testing**  

### **Run Unit Tests**  
```bash
dotnet test
```

### **Manual API Testing**  
📌 **Use Postman or Swagger UI** to:  
✅ **Create a user** → `/api/user (POST)`  
✅ **Fetch all users** → `/api/user (GET)`  
✅ **Delete a user** → `/api/user/{id} (DELETE)`  

---

## **🛠 Development & Debugging**  

### **Using Visual Studio**  
1. Open the solution in **Visual Studio**  
2. Set **Docker Compose** as the startup project  
3. Press **F5** to start debugging  

### **Manual Setup (Without Docker)**  
1. Start a MongoDB instance  
2. Update `appsettings.json` with the correct connection string  
3. Run the API manually:  
   ```bash
   cd UserService.Api
   dotnet run
   ```

---

## **🔒 Security Notes**  

🔹 **Default MongoDB credentials are for development only** – update them in production.  
🔹 **HTTPS is enabled by default** – ensure secure communications.  
🔹 **Use JWT authentication** (not included in this repo) for added security.  

---

## **🎯 Why Use User Service API?**  

✅ **Scalable & Efficient** – Built for **modern web applications and microservices**.  
✅ **Secure & Cloud-Ready** – Supports **Docker, Kubernetes, and AWS/Azure deployments**.  
✅ **Fast & Flexible** – Uses **MongoDB for high-speed data storage and retrieval**.  
✅ **Enterprise-Grade** – Implements **best practices for API design and security**.  

---

## **📜 License**  

This project is licensed under the **MIT License**. See [LICENSE](LICENSE) for details.  

---

## **📞 Contact**  

For feedback, contributions, or inquiries:  
📧 **Email**: [mreshboboyev@gmail.com](mailto:mreshboboyev@gmail.com)  
💻 **GitHub**: [MrEshboboyev](https://github.com/MrEshboboyev/user-service-with-mongo-db)  

---

🚀 **Scale your user management system with User Service API!** Clone the repo & start building today!  
