# PreventKids

> **Trabajo universitario.** Proyecto de curso de la Universidad Peruana de Ciencias
> Aplicadas (UPC), desarrollado en equipo de cinco estudiantes entre abril y mayo de 2026.
> No maneja datos reales de pacientes.

API REST de una plataforma para que familias y profesionales de la salud hagan seguimiento
del sobrepeso infantil: mediciones, alertas, ejercicios recomendados, contenido educativo,
consultas virtuales y un chat de apoyo.

Sitio publicado: https://prevent-kids.vercel.app

## Tecnologías

- Java 21 y Spring Boot 4
- Spring Data JPA con PostgreSQL
- Spring Security con autenticación JWT
- Documentación de la API con Swagger (springdoc-openapi)
- ModelMapper para los DTO

## Módulos

Usuarios y roles, distritos, mediciones, alertas y tipos de alerta, limitaciones físicas,
ejercicios recomendados, perfiles y especialidades de profesionales, contenido educativo,
consultas virtuales y chat.

## Cómo correrlo

Necesita una base PostgreSQL y estas variables de entorno:

```
DATABASE_URL=jdbc:postgresql://localhost:5432/preventkids
PGUSER=postgres
PGPASSWORD=tu_contraseña
JWT_SECRET=una_clave_larga_y_aleatoria
```

```
./mvnw spring-boot:run
```

La documentación queda en `http://localhost:8080/swagger-ui.html`.
