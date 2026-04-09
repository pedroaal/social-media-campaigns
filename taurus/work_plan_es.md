Bien. Ahora construiré para ti un plan de trabajo trimestral concreto vinculado a ese flujo de trabajo.

Pero primero—**crítica honesta**: Tu secuencia de flujo de trabajo está al revés.

Estás diciendo `[investigación_marca, investigación_mercado] -> análisis_marketing -> plan_trabajo`. Eso fluye *hacia afuera* desde el contexto del mercado. Pero en realidad necesitas fluir *hacia adentro* primero desde el problema del usuario, y luego validar con el contexto del mercado.

**Mejor secuencia:**

```
[Diagnóstico de Abandono] 
  -> [investigación_marca + investigación_mercado] 
    -> análisis_marketing 
      -> plan_trabajo
```

**¿Por qué?** Porque si haces la investigación de mercado *antes* de entender tu problema específico de abandono, estarás estudiando las cosas equivocadas. Podrías descubrir que los competidores tienen programas de lealtad, pero eso podría no abordar el factor real de deserción de *tu* gimnasio.

---

## Plan de Trabajo Trimestral: Causa Raíz → Soluciones Temporales

Estructuraré esto como **tres flujos integrados** que se alimentan entre sí y luego convergen en un plan de trabajo.

---

# **TRIMESTRE 1: DIAGNÓSTICO E INVESTIGACIÓN**

## **FLUJO A: Diagnóstico de Abandono (Semanas 1-6)**

### Semana 1-2: Auditoría de Datos

**Responsable:** Tú + 1 administrativo

**Entregable: Perfil de Deserción**

```
□ Extracción de datos históricos:
  ├─ Todos los miembros que abandonaron en los últimos 12 meses
  │  ├─ Fecha de inscripción → fecha de abandono (calcular LTV en días)
  │  ├─ Cohorte: ¿Cuántos se inscribieron en el mes X, cuántos siguen activos?
  │  └─ Segmentación: enfocados en clases vs. levantadores solos vs. multiservicio
  ├─ Instantánea de la base de miembros actual
  │  ├─ Total activos: 2,100
  │  ├─ Desglose por servicio (solo gimnasio vs. clases vs. pádel)
  │  └─ Distribución de compromiso (activos diarios vs. semanales vs. fantasma)
  └─ Impacto en los ingresos: ¿Qué segmento de deserción cuesta más?

□ Resultado: Gráfico de curva de abandono
  Ejemplo: "Mes 1: 5% abandono, Mes 2: 8%, Mes 3: 12%..."
           (te dice si la pérdida es inicial o gradual)
```

### Semana 3-4: Entrevistas a Ex-miembros (5 Porqués)

**Responsable:** Tú (puedes delegar en el administrativo para la programación)

**Objetivo: 15 miembros que abandonaron** (mureados aleatoriamente por fechas de abandono)

**Guion de entrevista (semiestructurado, 20-30 min)**

```
Apertura: "Notamos que cancelaste en [mes]. ¿Ayúdanos a entender por qué?"

Nivel 1 (Síntoma):
  P: "¿Cuál fue la razón principal por la que decidiste cancelar?"
  Nota: Probablemente sea superficial (precio, tiempo, aburrimiento, mudanza)

Nivel 2-3 (Profundizar):
  P: "¿Cuándo empezaste a sentirte así exactamente?"
  P: "¿Hubo algo que casi te hiciera quedarte?" (revela factores de retención)
  P: "¿Hubo un momento específico en que lo decidiste?"
  
Nivel 4-5 (Causa raíz):
  P: "¿Habías experimentado [problema superficial] antes o era algo nuevo?"
  P: "¿Qué te habría hecho quedarte?" (abre el espacio de posibilidades)
  P: "Si arregláramos [X], ¿volverías?"

Cierre:
  P: "¿Algún pensamiento final? ¿Algo que debamos saber?"
```

**En paralelo: Entrevistas a miembros activos (8-10 miembros comprometidos)**

```
Mismo guion pero invertido:
  "¿Qué te hace volver?"
  "¿Cuándo estuviste a punto de dejarlo?"
  "¿Qué te haría irte?"
→ Identifica anclas de retención (lo opuesto a los factores de deserción)
```

**Resultado: Personas de Abandono**

```
Ejemplo (ficticio):

PERSONA 1: "Principiante Motivado" (30% de la deserción)
  ├─ Comportamiento de inscripción: reclutado por un amigo, alta ilusión inicial
  ├─ Momento de abandono: Mes 2-3 (abandono temprano)
  ├─ Causa raíz: 
  │  ├─ Falta de retroalimentación sobre estructura/progresión
  │  ├─ Se siente perdido sin guía
  │  └─ No ve progreso (mentalidad: "estoy desperdiciando dinero")
  ├─ Factores de retención: volvería si tuviera evaluaciones 1:1, seguimiento de metas
  └─ Frecuencia: intentó ~2 veces/semana → lo dejó

PERSONA 2: "Entusiasta de Clases" (40% de la deserción)
  ├─ Comportamiento de inscripción: atraído por un instructor de clase específico
  ├─ Momento de abandono: Mes 4-6 (abandono a medio plazo)
  ├─ Causa raíz:
  │  ├─ El instructor se fue / el horario cambió / la clase se canceló
  │  ├─ Probó otras clases pero "no es lo mismo"
  │  └─ Perdió el hábito/vínculo con la comunidad
  ├─ Factores de retención: volvería si hubiera responsabilidad (desafío grupal), comunidad de clase alternativa
  └─ Frecuencia: 4-5 veces/semana → bajó a 0

PERSONA 3: "Cambiador de Estilo de Vida" (30% de la deserción)
  ├─ Momento de abandono: Mes 6-12 (abandono tardío)
  ├─ Causa raíz: 
  │  ├─ Cambio de trabajo, mudanza, situación familiar, lesión
  │  └─ El gimnasio no es adaptable (sin opción remota, sin enfoque en recuperación)
  ├─ Factores de retención: volvería si tuviera flexibilidad (opción de pausa, ejercicios en casa), clases de recuperación más ligeras
  └─ Frecuencia: 3-4 veces/semana → conflicto vital
```

### Semana 5-6: Síntesis de Datos

**Responsable:** Tú

**Resultado: Matriz de Hipótesis de Causa Raíz**

```
Factor de Abandono            % de Deserción   Gravedad    Capacidad de abordar
─────────────────────────────────────────────────────────────────────────────
Falta de feedback de progreso 35%              Alta        Alta
Interrupción de la rutina     25%              Alta        Media
Dependencia entrenador/clase  20%              Media       Media
Sensibilidad al precio        12%              Baja        Baja
Problemas de instalaciones    8%               Baja        Media

→ Áreas de enfoque: los 3 principales factores representan el 80% de la deserción
```

---

## **FLUJO B: Investigación de Marca (Semanas 3-8)**

**Responsable:** Tú (puedes contratar a un freelancer para las encuestas si hay presupuesto)

### Semana 3-5: Estudio de Percepción de Miembros

**Método:** Breve encuesta online (5 min) + entrevistas de profundidad

**Encuesta (distribuir a 100 miembros activos)**

```
P1: "¿Por qué te uniste a Taurus?" (elige las 3 principales)
    [ ] Entrenadores / experiencia
    [ ] Variedad de clases
    [ ] Equipo / instalaciones
    [ ] Comunidad / social
    [ ] Ubicación
    [ ] Precio
    [ ] Otro: ___

P2: "¿Cómo describirías a Taurus a un amigo?"
    (Texto abierto - revela percepción de marca)

P3: "¿En qué es mejor Taurus?"
    [ ] Entrenamiento de fuerza
    [ ] Clases / fitness grupal
    [ ] Comunidad / motivación
    [ ] Entrenamiento apto para principiantes
    [ ] Otro: ___

P4: "¿Qué podría mejorar Taurus?"
    (Texto abierto)

P5: "¿Qué tan probable es que recomiendes a un amigo?" 
    (1-10 estilo NPS)
```

**Resultado: Mapa de Posicionamiento de Marca**

```
Percepción Actual vs. Posición Deseada:

HOY (según encuestas):
  ✓ "Lugar para levantadores serios" (80% menciona entrenadores/fuerza)
  ✓ "Buen equipo"
  ✗ "No es apto para principiantes"
  ✗ "Se siente intimidante"
  ✗ "Sin espíritu de comunidad"
  ✗ "Las clases se sienten separadas del gimnasio principal"

PERSPECTIVA: Taurus se percibe como un "gimnasio dependiente de entrenadores para usuarios avanzados"
             pero tus datos de deserción muestran que los principiantes + gente de clases se están yendo.
             
OPORTUNIDAD: Reposicionar de "fuerza seria" a "progresión accesible"
             (atraer a tus Personas 1 y 2, reducir la intimidación para la Persona 1)
```
