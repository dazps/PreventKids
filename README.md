# PreventKids

> **Trabajo universitario.** Proyecto de curso de la Universidad Peruana de Ciencias
> Aplicadas (UPC), desarrollado en equipo de cinco estudiantes en 2026.
> No maneja datos reales de pacientes.

Plataforma web para que familias y profesionales de la salud hagan seguimiento
del sobrepeso infantil: mediciones, alertas, ejercicios recomendados, contenido educativo,
consultas virtuales y un chat de apoyo con IA.

- Sitio: https://prevent-kids.vercel.app
- API: https://preventkids.onrender.com

## Estructura

- `backend/`: API REST en Spring Boot
- `frontend/`: aplicación en Angular
- `scripts/`: datos de prueba en SQL

## Tecnologías

- Angular 21 en el frontend, publicado en Vercel
- Java 21 y Spring Boot 4 en el backend, publicado en Render con Docker
- Spring Data JPA con PostgreSQL
- Spring Security con autenticación JWT
- Documentación de la API con Swagger (springdoc-openapi)
- ModelMapper para los DTO
- Chat con la API de Gemini

## Módulos

Usuarios y roles, distritos, mediciones, alertas y tipos de alerta, limitaciones físicas,
ejercicios recomendados, perfiles y especialidades de profesionales, contenido educativo,
consultas virtuales y chat.

## Cómo correrlo

Backend: necesita una base PostgreSQL y estas variables de entorno.

```
DATABASE_URL=jdbc:postgresql://localhost:5432/preventkids
PGUSER=postgres
PGPASSWORD=tu_contraseña
GEMINI_API_KEY=tu_clave   # opcional, para el chat
```

```
cd backend
./mvnw spring-boot:run
```

Frontend:

```
cd frontend
npm install
npm start
```

La documentación queda en `http://localhost:8080/swagger-ui.html`.
