# API de Artículos

CRUD de artículos desarrollado con **Java**, **Spring Boot** y **MySQL**, con un front sencillo en HTML y JavaScript.

**Autor: ABEL SEBASTIAN TINTILAY**
**Curso: C26223 | Back-End / Java | Jueves - 19 a 21 hs**

## Video explicativo

[Ver video del funcionamiento de la API con Postman y la base de datos](PEGAR_AQUI_EL_LINK)

## Tecnologías

- Java 17 o superior
- Spring Boot 3.2.5 (Spring Web y Spring Data JPA)
- MySQL (con XAMPP)
- Maven
- Postman (para probar la API)
- HTML, CSS y JavaScript (front)

## Estructura del proyecto

```
articulo-api-mysql-funcional
├── pom.xml
├── README.md
├── src/main/java/com/ejemplo/articulos
│   ├── ArticuloApiApplication.java   (clase principal)
│   ├── controller/                   (endpoints REST)
│   ├── service/                      (lógica de negocio)
│   ├── repository/                   (acceso a datos con JPA)
│   └── model/                        (entidad Articulo)
├── src/main/resources/application.properties
└── frontend/index.html               (interfaz web)
```

## Requisitos

- JDK 17 o superior
- XAMPP (módulo MySQL)
- VS Code con el Extension Pack for Java (o cualquier IDE para Java)
- Postman (opcional, para probar los endpoints)

## Cómo ejecutarlo

1. Abrir **XAMPP** e iniciar **MySQL**.
2. Crear la base de datos `articulos_db` (por ejemplo desde `http://localhost/phpmyadmin`, con cotejamiento `utf8mb4_general_ci`). La tabla `articulo` la crea automáticamente JPA al iniciar la aplicación.
3. Revisar la conexión en `src/main/resources/application.properties` (por defecto usuario `root` sin contraseña, como en XAMPP):

4. Ejecutar la clase `ArticuloApiApplication` (botón **Run** en VS Code).
5. Verificar que la API responde en `http://localhost:8080/api/articulos`.
6. Abrir `frontend/index.html` en el navegador.