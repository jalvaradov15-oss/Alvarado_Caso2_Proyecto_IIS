# PROPUESTA DE MANTENIMIENTO

## PROYECTO: AGENDA PERSONAL DE CITAS

---

## 1\. INFORMACIÓN GENERAL

**Proyecto:** Agenda Personal de Citas  
**Versión:** 2.0  
**Fecha:** 18 de noviembre de 2025  
**Elaborado por:** \[Anthony Cano]

---

## 2\. INTRODUCCIÓN

Este documento presenta las propuestas de mantenimiento identificadas para el sistema de Agenda Personal de Citas, clasificadas en tres categorías: correctivo, adaptativo y perfectivo.

---

## 3\. MANTENIMIENTO CORRECTIVO

### 3.1 Problema Identificado

**ID:** MC-01  
**Título:** Notificaciones no funcionan en modo ahorro de energía  
**Severidad:** Alta  
**Prioridad:** Crítica

**Descripción del Problema:**  
Los usuarios reportan que las notificaciones de recordatorio no se muestran cuando el dispositivo está en modo de ahorro de energía o la aplicación está en segundo plano.

**Impacto:**

* Usuarios pierden citas importantes
* Disminuye la confianza en la aplicación
* Afecta al 60% de los usuarios móviles

**Causa Raíz:**  
El servicio de notificaciones se detiene cuando el sistema operativo limita los procesos en segundo plano para ahorrar batería.

**Solución Propuesta:**

1. Implementar servicio persistente en segundo plano
2. Utilizar WorkManager para programación confiable
3. Solicitar permisos especiales para ejecutar en segundo plano
4. Implementar notificaciones programadas del sistema

**Recursos Necesarios:**

* 1 desarrollador Android/iOS
* 80 horas de desarrollo
* 20 horas de pruebas

**Tiempo Estimado:** 2 semanas

**Costo Estimado:** $2,000 USD

**Plan de Implementación:**

* Semana 1: Desarrollo e implementación
* Semana 2: Pruebas y despliegue

---

## 4\. MANTENIMIENTO ADAPTATIVO

### 4.1 Cambio Requerido

**ID:** MA-01  
**Título:** Integración con Google Calendar y Outlook  
**Prioridad:** Media  
**Justificación:** Sincronización con calendarios corporativos

**Descripción del Cambio:**  
Implementar sincronización bidireccional con Google Calendar y Microsoft Outlook para permitir a los usuarios gestionar todas sus citas desde una sola aplicación.

**Motivación:**

* 75% de usuarios utilizan calendarios corporativos
* Competencia ya ofrece esta funcionalidad
* Solicitud frecuente de usuarios empresariales

**Funcionalidades a Implementar:**

1. Autenticación OAuth con Google y Microsoft
2. Importación de citas existentes
3. Sincronización automática bidireccional
4. Manejo de conflictos de sincronización
5. Configuración de calendarios a sincronizar

**Beneficios:**

* Mayor adopción en entornos corporativos
* Eliminación de duplicación de tareas
* Centralización de información
* Ventaja competitiva

**Recursos Necesarios:**

* 2 desarrolladores backend
* 1 desarrollador frontend
* 160 horas de desarrollo
* 40 horas de pruebas

**Tiempo Estimado:** 4 semanas

**Costo Estimado:** $5,000 USD

**Riesgos:**

* Cambios en APIs de terceros
* Problemas de seguridad y privacidad
* Complejidad en manejo de conflictos

**Plan de Mitigación:**

* Usar librerías oficiales y mantenidas
* Implementar encriptación end-to-end
* Desarrollar algoritmo robusto de resolución de conflictos

---

## 5\. MANTENIMIENTO PERFECTIVO

### 5.1 Mejora Propuesta

**ID:** MP-01  
**Título:** Implementar vista de timeline para visualización de citas  
**Prioridad:** Baja  
**Tipo:** Mejora de interfaz

**Descripción de la Mejora:**  
Agregar una nueva vista de timeline que muestre las citas en una línea de tiempo visual e interactiva, similar a un diagrama de Gantt.

**Justificación:**

* Mejora la experiencia visual del usuario
* Facilita la identificación de períodos libres
* Permite mejor planificación del día
* Diferenciación de la competencia

**Características:**

1. Vista de timeline por día/semana
2. Bloques visuales proporcionales a la duración
3. Código de colores por categoría
4. Arrastrar y soltar para reprogramar
5. Zoom in/out para diferentes niveles de detalle

**Beneficios:**

* Interfaz más moderna y atractiva
* Mejor comprensión visual del calendario
* Facilita la gestión de tiempo
* Aumenta satisfacción del usuario

**Recursos Necesarios:**

* 1 diseñador UX/UI
* 1 desarrollador frontend
* 120 horas de desarrollo
* 30 horas de pruebas de usabilidad

**Tiempo Estimado:** 3 semanas

**Costo Estimado:** $3,500 USD

**Métricas de Éxito:**

* Aumento del 20% en tiempo de uso de la app
* Reducción del 15% en citas reprogramadas
* Puntuación de satisfacción > 4.5/5

---

## 6\. RESUMEN DE PROPUESTAS

| ID    |    Tipo    | Título                              | Prioridad | Tiempo | Costo  |
|-------|------------|-------------------------------------|-----------|--------|--------|
| MC-01 | Correctivo | Notificaciones en ahorro de energía | Alta      | 2 sem  | $2,000 |
| MA-01 | Adaptativo | Integración Google/Outlook          | Media     | 4 sem  | $5,000 |
| MP-01 | Perfectivo | Vista timeline                      | Baja      | 3 sem  | $3,500 |

**Costo Total:** $10,500 USD  
**Tiempo Total:** 9 semanas

---

Mes 1:  
Semanas 1-2: MC-01 (Correctivo - Notificaciones)

Mes 2:  
Semanas 3-6: MA-01 (Adaptativo - Integraciones)

Mes 3:  
Semanas 7-9: MP-01 (Perfectivo - Timeline)

---

## 8\. RECOMENDACIONES

1. **Priorizar MC-01:** Es crítico para la funcionalidad básica
2. **Evaluar ROI de MA-01:** Antes de invertir en integraciones
3. **Realizar pruebas A/B de MP-01:** Para validar adopción

---

## 9\. CONCLUSIONES

Las tres propuestas de mantenimiento abordan diferentes aspectos del sistema:

* **Correctivo:** Garantiza funcionalidad básica
* **Adaptativo:** Expande capacidades y mercado
* **Perfectivo:** Mejora experiencia del usuario

Se recomienda implementarlas en el orden propuesto para maximizar valor y minimizar riesgos.

---

**Elaborado por:** \[Anthony Cano]  
**Fecha:** 18/11/2025  
**Versión:** 1.0

