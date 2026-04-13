# ADR-001: Uso de Clean Architecture

## Estado
Aceptado

## Contexto
Se requiere una arquitectura que permita separar lógica de negocio, infraestructura y exposición HTTP.

## Decisión
Se adopta Clean Architecture con capas: Domain, Application, Infrastructure y API.

## Consecuencias
✔ Bajo acoplamiento  
✔ Alta testabilidad  
❌ Mayor complejidad inicial
