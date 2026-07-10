# Spring Boot Product Service

A RESTful Product Service built using Spring Boot. This microservice manages product information using Spring Data JPA and an H2 in-memory database.

## 🚀 Features

- Add new products
- Retrieve product details
- RESTful API
- Spring Data JPA integration
- H2 In-Memory Database
- Layered Architecture
- Maven Project

## 🛠️ Tech Stack

- Java 17
- Spring Boot
- Spring Web
- Spring Data JPA
- H2 Database
- Maven

## 📁 Project Structure

```
src
├── main
│   ├── java
│   │   └── com.skillfirstlab.productservice
│   │       ├── Controller
│   │       ├── Entity
│   │       ├── Repository
│   │       ├── Service
│   │       └── ProductServiceApplication.java
│   └── resources
│       └── application.properties
```

## ⚙️ Configuration

Application URL:

```
http://localhost:8081
```

### H2 Database

```
Database : productdb
Username : sa
Password : (empty)
```

JDBC URL

```
jdbc:h2:mem:productdb
```

H2 Console

```
http://localhost:8081/h2-console
```

## 📌 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/product/save` | Create a new product |
| GET | `/product/{id}` | Get product by ID |
| GET | `/product/all` | Get all products |
| PUT | `/product/update/{id}` | Update product |
| DELETE | `/product/delete/{id}` | Delete product |

> **Note:** Keep only the endpoints that are implemented in your project.

## 📥 Sample Request

```json
{
  "productName": "Laptop",
  "productPrice": 65000,
  "productCategory": "Electronics"
}
```

## 📤 Sample Response

```json
{
  "id": 1,
  "productName": "Laptop",
  "productPrice": 65000,
  "productCategory": "Electronics"
}
```

## ▶️ Running the Project

Clone the repository:

```bash
git clone https://github.com/your-username/Spring-Boot-Api-ProductService.git
```

Navigate to the project folder:

```bash
cd Spring-Boot-Api-ProductService
```

Run the application:

```bash
mvn spring-boot:run
```

Or run the `ProductServiceApplication` class directly from your IDE.

## 📦 Dependencies

- Spring Boot Starter Web
- Spring Boot Starter Data JPA
- H2 Database
- Spring Boot Starter Test

## 👨‍💻 Author

**Ashwin V**

Computer Science Engineering Student

---

⭐ If you found this project useful, please consider giving it a **Star** on GitHub.
