# README - Cambios aplicados en Power Query

Archivo asociado: PerezTovar_TomasAlejandro.pbix

## Descripción

Este README documenta los cambios efectivos que realizaste en Power Query sobre la tabla original de solicitudes de visas. El objetivo es dejar registro claro y reproducible de las transformaciones aplicadas.

## Resumen de cambios aplicados

### 1. Renombrado de columnas

- Año Expedición  → Año
- Mes Expedición  → Mes
- Nacionalidad    → País
- Tipo Documento  → TipoVisa
- Número          → Cantidad

Las columnas Sexo y Edad se mantuvieron con sus nombres originales.

### 2. Cambio de tipos de datos

- Año: tipo entero
- Mes: tipo texto (ahora contiene el nombre del mes, p. ej. "enero")
- País: texto
- Sexo: texto
- Edad: entero
- TipoVisa: texto
- Cantidad: entero

### 3. Reemplazo de valores en la columna Mes

En vez de números (1, 2, 3, ...) la columna Mes ahora contiene el nombre del mes en español. Mapeo usado:

- 1 → enero
- 2 → febrero
- 3 → marzo
- 4 → abril
- 5 → mayo
- 6 → junio
- 7 → julio
- 8 → agosto
- 9 → septiembre
- 10 → octubre
- 11 → noviembre
- 12 → diciembre

### 4. Corrección puntual de nacionalidad

Se corrigió un error de digitalización en el nombre del país: "ESPA¥A" → "ESPAÑA".
