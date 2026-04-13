# ADR-005: Estrategia de testing

## Estado
Aceptado

## Contexto

El sistema requiere validación automatizada para garantizar la calidad del código, evitar regresiones y facilitar la evolución del sistema.

## Decisión

Se adopta una estrategia híbrida de testing:

### Unit tests
- Capa Application
- Uso de mocks o NullLogger
- Validación de lógica de negocio

### Integration tests
- Capa Infrastructure
- Uso de EF Core InMemory
- Validación de persistencia

## Justificación

- Permite aislar lógica de negocio
- Reduce dependencia de base de datos real
- Mejora velocidad de ejecución en CI

## Consecuencias

✔ Alta cobertura de lógica crítica  
✔ Tests rápidos y reproducibles  
✔ Separación clara de responsabilidades  

❌ EF InMemory no replica completamente SQL Server  
❌ Requiere mantener datos de prueba (seed)  
