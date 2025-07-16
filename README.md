<div align="left">
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="MIT-license">
  <img src="https://img.shields.io/badge/Java-21-blue.svg" alt="Java-version">
  <img src="https://img.shields.io/github/issues/devgabrieljeronimo/first-spring-aplication" alt="Issues">

<div/>
  
# 📦 First Spring Application

<div align="center">
  My first projetc using Spring, it's a simple model of a API RESTful that implements CRUD(Create, Read, Update, Delete) with products.
</div>

<br/>

## 🚀 Technologies used

- Java 21
- Spring Boot
- Spring Web
- Spring Data JPA
- Spring DevTools
- Flyway
- PostgreSQL
- Maven

<br/>

## ⚙️ How to run the project

1. Clone the repository:

```bash
git clone https://github.com/devgabrieljeronimo/first-spring-aplication.git
```

<br/>

2. Create a PostgreSQL database, like this:

```sql
CREATE DATABASE product-api;
```
If you don't have the PostgreSQL, you can download [here](https://www.postgresql.org/download/).

<br/>

3. Open the project in an IDE(Intellij, Eclipse, NetBeans).

<br/>

4. Open the ```application-example.properties``` in:

```css
src/main/resources/application-example.properties
```
Rename to ```application.properties```, and put your database url, username and password, inside the file exist more instructions.

<br/>

5. If you already finished all, you can run the project.
   
    note: you don't need to create a table for products, the FlyWay will do it for you.

<br/>

## 📬 Endpoints of the API

Below you can see every endpoint of my project:
| Method    | Route           | Description                   |
|-----------|-----------------|-------------------------------|
| GET       | /products       | List every products           |
| GET(byID) | /products/{id}  | List a product                |
| POST      | /products       | Create a new product          |
| PUT       | /products/{id}  | Update a product existing     |
| DELETE    | /products/{id}  | Delete a product              |

You can test the endpoints with [Insomnia](https://insomnia.rest/download) or [Postman](https://www.postman.com/downloads/).

<br/>

## 🗃️ Flyway migrations

Flyway is a tool that versions and updates the database automatically with SQL scripts.

The migrations stay on the paste:
```css
src/main/resources/db/migration/
```

The project will starts with V1__create-table-product.sql:
```sql
CREATE TABLE product (
  id SERIAL PRIMARY KEY,
  name VARCHAR(255) NOT NULL,
  price BIGINT NOT NULL
);
```

<br/>

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/devgabrieljeronimo/first-spring-aplication/blob/main/LICENSE) file for details.

<br/>

## 🙋‍♂️ Owner
Gabriel Jeronimo

GitHub: [@devgabrieljeronimo](https://github.com/devgabrieljeronimo)
