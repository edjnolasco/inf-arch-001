# ADR-004: Uso de Docker para contenerización

## Estado
Aceptado

## Contexto

Se requiere una forma consistente de ejecutar la aplicación en distintos entornos (desarrollo, integración y potencial despliegue), evitando problemas de configuración local, dependencias y versiones de runtime.

## Decisión

Se adopta Docker para:

- Contenerizar la API ASP.NET Core
- Ejecutar SQL Server en contenedor
- Orquestar servicios mediante docker-compose

## Justificación

- Permite reproducibilidad del entorno
- Simplifica onboarding de nuevos desarrolladores
- Facilita integración con CI/CD
- Permite transición futura a despliegues en nube (Azure / AWS)

## Consecuencias

✔ Entorno consistente entre desarrollo y CI  
✔ Aislamiento de dependencias  
✔ Base para despliegue en contenedores  

❌ Requiere conocimiento adicional de Docker  
❌ Incrementa complejidad inicial del proyecto  
