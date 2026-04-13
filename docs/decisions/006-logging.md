# ADR-006: Estrategia de logging

## Estado
Aceptado

## Contexto

Se requiere visibilidad sobre el comportamiento del sistema para facilitar debugging, monitoreo y trazabilidad de operaciones.

## Decisión

Se utiliza `ILogger<T>` en la capa Application (servicios) para registrar eventos relevantes.

## Alcance del logging

- Operaciones CRUD
- Validaciones fallidas
- Conflictos (duplicados)
- Errores controlados

## Justificación

- Integración nativa con ASP.NET Core
- Bajo costo de implementación
- Extensible a sistemas de observabilidad

## Consecuencias

✔ Trazabilidad básica del sistema  
✔ Preparación para observabilidad avanzada  
✔ Integración con herramientas externas  

❌ No incluye aún correlación distribuida  
❌ No hay métricas ni tracing implementados (fase futura)  
