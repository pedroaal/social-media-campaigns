# TAURUS GYM: Flujo de Trabajo de Estrategia Operativa y Competitiva Multi-Agente

## Prompt de Ultrapilot para Oh My ClaudeCode

---

## CONTEXTO

**Cliente:** Taurus Gym, Manta, Ecuador
**Ubicación:** Manta, segmento de ingresos medios-altos
**Estado Actual:**

- Usuarios mensuales: ~2,100
- Tasa de abandono de miembros: 18%
- Personal: ~10 entrenadores, ~10 entrenadores especializados, ~10 empleados de apoyo (administración, limpieza, seguridad)
- Instagram: @taurusgymmanta

**Objetivos (horizonte de 6 meses):**

1. Reducir el abandono del 18% → 5%
2. Aumentar los usuarios mensuales de 2,100 → 2,500
3. Identificar y abordar las causas raíz operativas
4. Desarrollar un plan de acción por fases (Semanas 1-4 = victorias rápidas; Semanas 5-12 = mediano plazo; Q2 2026 = cambios estructurales)

**Causas Raíz (validadas mediante auditoría de miembros):**

1. Hacinamiento durante las horas pico
2. Servicio y limpieza deficientes
3. Seguimiento inadecuado de los entrenadores
4. Monopolización de entrenadores privados (máquinas/control de acceso)

**Restricción de Presupuesto:** <$1,000 para las Semanas 1-4 (solo personal + procesos; sin nueva tecnología)
**Prioridad del Cronograma:** Enfoque inmediato en el hacinamiento; monopolización diferida al Q2

**Competidores (Manta, segmento medio-alto):**

- Master Gym (@mastergym.87)
- King World Gimnasio / King CF
- MANTA CrossFit / Satori Cross
- Super Saya Gym
- Gimnasio Vida Plena

---

## ARQUITECTURA DEL FLUJO DE TRABAJO

**Etapa 1 (Paralela):**

- Agente A: soluciones_operativas:opus
- Agente B: auditoria_marketing_competencia:sonnet

**Etapa 2 (Secuencial):**

- Agente C: estratega_sintesis:opus

**Etapa 3 (Secuencial):**

- Agente D: plan_trabajo_fases:sonnet

---

## AGENTE A: SOLUCIONES OPERATIVAS (Modelo: Claude Opus)

### Tarea

Generar soluciones concretas y accionables para cada una de las cuatro causas raíz. Priorizar por:

1. Cronograma (¿qué es implementable en <$1K, Semanas 1-4?)
2. Factibilidad de recursos (capacidad del personal existente)
3. Impacto en el miembro (mejora esperada en la retención)

### Datos de Entrada

- Causas raíz (según la lista anterior)
- Composición del personal: 10 entrenadores, 10 entrenadores especializados, 10 empleados de apoyo
- Presupuesto: <$1,000 para las Semanas 1-4
- Instagram de Taurus: @taurusgymmanta
- Métrica de éxito: Reducción en la tasa de quejas en horas pico + medida a través de encuestas de seguimiento

### Formato de Salida

Para cada causa raíz, proporcionar:

```
## Causa Raíz: [Nombre]

### Declaración del Problema
[1-2 oraciones explicando el impacto observado en los miembros]

### Solución 1: [Nombre] | Cronograma: [Semanas 1-4 / Semanas 5-12 / Q2] | Presupuesto: $[X] | Dificultad: [Baja/Media/Alta]
[2-3 oraciones describiendo la solución]
- **Pasos de implementación:** [Lista de puntos, máx. 4 puntos]
- **Responsable:** [¿Qué rol: entrenador, gerente, personal administrativo?]
- **Métricas a seguir:** [¿Cómo medir el éxito?]

### Solución 2: [Formato similar]

### Solución 3: [Formato similar]

### Recomendación Prioritaria
[1 oración sobre qué solución pilotear primero y por qué]
```

### Restricciones

- Asumir que no hay nuevas contrataciones en las Semanas 1-4.
- Asumir que el personal existente puede absorber de 5 a 10 horas/semana de trabajo en nuevos procesos.
- NO sugerir soluciones tecnológicas pagas (presupuesto de capacitación <$1K).
- Todas las soluciones deben ser reversibles si los datos muestran que no están funcionando.

---

## AGENTE B: AUDITORÍA DE MARKETING DE LA COMPETENCIA (Modelo: Claude Sonnet)

### Tarea

Investigar los gimnasios competidores enumerados y extraer:

1. **Cómo se posicionan/comunican** su gimnasio (propuestas de valor, grupos demográficos objetivo, puntos de dolor que abordan).
2. **Canales de marketing y contenido** (estrategia de Instagram, temas de los mensajes, frecuencia, tácticas de interacción).
3. **Cómo abordan cada causa raíz** (ej.: ¿cómo comunican las soluciones al hacinamiento, la limpieza, la accesibilidad de los entrenadores?).

### Datos de Entrada

- Objetivo de Taurus: ingresos medios-altos, edades 30–50, locales de Manta.
- Competidores a auditar: Master Gym (@mastergym.87), King World Gimnasio, MANTA CrossFit, Super Saya Gym, Gimnasio Vida Plena.
- Enfoque: Mensajes de marketing que se alineen con los problemas operativos de Taurus.

### Formato de Salida

```
## Resumen del Análisis de la Competencia

### [Nombre del Competidor] | Instagram: [@usuario]

#### Posicionamiento y Propuestas de Valor
[2-3 oraciones sobre cómo se posicionan: "fuerza", "comunidad", "entrenadores expertos", etc.]

#### Temas de Marketing
- Tema 1: [¿Qué problema/deseo resaltan en las publicaciones? Ej.: "transformación", "seguridad", "guía experta"]
- Tema 2: [Otro tema clave]
- Tema 3: [Otro tema clave]

#### Estrategia de Contenido
- Frecuencia: [Publicaciones por semana, cadencia típica]
- Tipos de contenido: [Ej.: transformaciones de miembros, consejos de entrenadores, recorridos por las instalaciones, resúmenes de clases]
- Ganchos de interacción: [Llamadas a la acción, tácticas de participación comunitaria]

#### Cómo Abordan los Puntos de Dolor de Taurus
- **Hacinamiento:** [Si es visible, ¿cómo comunican la disponibilidad/variedad de clases?]
- **Limpieza:** [¿Muestran el mantenimiento/higiene de las instalaciones?]
- **Seguimiento del entrenador:** [¿Enfatizan la accesibilidad del entrenador o el asesoramiento personalizado?]
- **Monopolización de entrenadores:** [¿Resaltan el acceso justo a los equipos/entrenadores?]

#### Perspectivas para Taurus
[1-2 oraciones sobre lo que Taurus podría aprender o cómo diferenciarse de este competidor]

---

### Perspectivas Entre Competidores

#### Brechas que Taurus Puede Llenar
[2-3 oraciones sobre áreas donde los competidores son débiles y Taurus puede diferenciarse]

#### Temas Comunes en los Mensajes
[¿Qué enfatizan todos los competidores? (ej.: "transformación", "comunidad", "resultados")]

#### Posicionamiento Recomendado para Taurus
[1-2 oraciones sobre la propuesta de valor única que Taurus debería apropiarse basada en el análisis competitivo]
```

### Restricciones

- Centrarse en la información pública (Instagram, Facebook, sitio web si está disponible).
- Si el Instagram de un competidor es privado o mínimo, fótalo y no especules.
- Distinguir entre mensajes "inferidos" y "observados".

---

## AGENTE C: ESTRATEGA DE SÍNTESIS (Modelo: Claude Opus)

### Tarea

Sintetizar los resultados del Agente A (soluciones operativas) + Agente B (perspectivas de la competencia) en una dirección estratégica cohesiva.

### Entrada

- Resultado del Agente A: 3 soluciones por causa raíz, con cronogramas/presupuestos/dificultad.
- Resultado del Agente B: Posicionamiento de la competencia + temas de mensajes + brechas identificadas.

### Formato de Salida

```
## Síntesis Estratégica: Posicionamiento Competitivo y Fases de Taurus

### Semanas 1-4: Victorias Rápidas (Movimientos de bajo costo y alta credibilidad)
[Sintetizar qué soluciones del Agente A encajan en el presupuesto + cronograma. Para cada una, anotar:]
- **Solución:** [Nombre del Agente A]
- **Por qué primero:** [Por qué esto genera impulso / aborda el dolor más urgente]
- **Impacto esperado en el miembro:** [Mejora estimada en la retención/satisfacción]
```
