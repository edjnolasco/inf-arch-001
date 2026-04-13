# ADR-003: Uso de ServiceResult

## Estado
Aceptado

## Contexto
Se necesita estandarizar respuestas y evitar excepciones como flujo.

## Decisión
Se implementa ServiceResult<T> y ServiceErrorType.

## Consecuencias
✔ Respuestas consistentes  
✔ Control de errores  
❌ Más código boilerplate
