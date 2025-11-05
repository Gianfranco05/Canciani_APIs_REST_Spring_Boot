# 🛍️ API REST de Gestión de Productos - Canciani

## 📝 Descripción del Proyecto
Este proyecto es una **API REST** desarrollada con **Spring Boot** para la gestión de productos de un sistema de e-commerce básico.  
Permite **crear, listar, actualizar, filtrar y eliminar productos**, aplicando **arquitectura en capas**, **DTOs**, **validaciones**, **manejo centralizado de errores** y persistencia en **H2 Database**.  
La API está documentada con **Swagger/OpenAPI** para pruebas interactivas de todos los endpoints.

---

## ⚙️ Tecnologías Utilizadas
- Java 21  
- Spring Boot 3.x  
- Spring Web  
- Spring Data JPA  
- H2 Database  
- Bean Validation  
- Lombok  
- Swagger/OpenAPI (springdoc)  
- Gradle  

---

## 🚀 Cómo Clonar y Ejecutar el Proyecto

```bash
git clone https://github.com/tu-usuario/productos-api.git
cd productos-api
```
Ejecutar el proyecto con Gradle
```bash
./gradlew bootRun    # Linux/Mac
gradlew.bat bootRun  # Windows
```
La aplicación se ejecutará en:
👉 http://localhost:8080

## 🌐 Endpoints de la API

| Método | Ruta | Descripción |
|--------|-------|-------------|
| GET | /api/productos | Listar todos los productos |
| GET | /api/productos/{id} | Obtener producto por ID |
| GET | /api/productos/categoria/{categoria} | Filtrar productos por categoría |
| POST | /api/productos | Crear un nuevo producto (DTO validado) |
| PUT | /api/productos/{id} | Actualizar un producto completo |
| PATCH | /api/productos/{id}/stock | Actualizar solo el stock |
| DELETE | /api/productos/{id} | Eliminar un producto |

## 📚 Acceso a Swagger UI
Swagger UI permite probar todos los endpoints de forma interactiva.

URL: http://localhost:8080/swagger-ui/index.html

## 🖥️ Acceso a la Consola H2
- URL: http://localhost:8080/h2-console

- JDBC URL: jdbc:h2:mem:productosdb

- User: sa

- Password: (vacío)

## 📸 Capturas de Pantalla
- Swagger UI mostrando la documentación completa
<img width="896" height="606" alt="image" src="https://github.com/user-attachments/assets/c9814c62-4ea8-4c8b-b1a1-dd2131543d76" />

- POST exitoso creando producto
<img width="666" height="789" alt="image" src="https://github.com/user-attachments/assets/359c29b2-be4a-400d-97a9-8ee9fff40cd6" />

- GET listando productos y filtrando por categoría
<img width="881" height="857" alt="image" src="https://github.com/user-attachments/assets/dee32079-392a-4e41-a77f-25be455ec386" />

- Error 404 cuando el producto no existe
<img width="750" height="653" alt="image" src="https://github.com/user-attachments/assets/9a5de02f-f31c-4353-8be6-2271f7f06961" />

- Error 400 por validación fallida
<img width="645" height="779" alt="image" src="https://github.com/user-attachments/assets/a98ff6f1-259d-459c-a935-77673d853ec1" />


## 👤 Autor
#### Nombre: Gianfranco Canciani
#### Legajo: 52611
#### DNI: 46866563
