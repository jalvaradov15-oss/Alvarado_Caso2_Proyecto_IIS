## Agenda Personal de Citas 

### 1. Documento de Requerimientos de Software (DRS)

El proyecto "Agenda Personal de Citas" fue elaborado por **Anthony Geovanny Cano Armijos** para la **Universidad Estatal de Milagro (UNEMI)**.

#### Propósito y Alcance
El propósito principal es servir como una herramienta digital eficiente para **gestionar, programar y recibir recordatorios de citas y eventos personales**. El alcance incluye crear, editar, eliminar y buscar citas, mostrar el calendario y configurar el recordatorio. No se incluyen funciones como el control de inventario o la compartición de calendarios.

#### Requerimientos Funcionales (RF)
* **Creación de Citas (RF1):** Incluir campos para fecha, hora, descripción/motivo, datos personales y lugar.
* **Visualización de Calendario (RF2):** Mostrar vista de calendario (diaria, semanal, mensual).
* **Edición y Eliminación (RF3):** Modificar cualquier detalle o eliminar una cita por completo.
* **Configuración de Recordatorio (RF4):** Permitir configurar una notificación o alarma en un tiempo predeterminado.
* **Búsqueda y Filtro (RF5):** Buscar por palabras clave o filtrar por contacto y rango de fechas.

#### Requerimientos No Funcionales (RNF)
* **Portabilidad (RNF1):** Compatible y funcional en **iOS, Android** y navegador web.
* **Rendimiento de Carga (RNF2):** La vista semanal (con hasta 50 citas) no debe tardar **más de 2 segundos** en cargarse.
* **Seguridad de Datos (RNF3):** Citas y datos personales deben estar **cifrados** y protegidos mediante inicio de sesión seguro.

---

### 2. Validación del Sistema y Casos de Prueba

La validación se realiza mediante Casos de Prueba (Unitarios y de Validación) para demostrar que el sistema cumple con lo prometido.

* **CP01 (RF1):** Prueba que la cita creada se guarde y se muestre en el calendario.
* **CP02 (RF4):** Verifica que se genere la notificación audible o visual 30 minutos o 1 hora antes de la cita.
* **CP03 (RNF1):** Valida que el intento de inicio de sesión con credenciales incorrectas sea denegado (Acceso Único/Seguridad).
* **CP04 (RNF2):** Mide la velocidad de sincronización, esperando que el proceso se complete en un tiempo **máximo de 3 segundos** entre dispositivos.
* **CP05 (RF5):** Confirma que una búsqueda por palabra clave ("dentista") solo retorne la cita que la contenga.

---

### 3. Propuesta de Mantenimiento

Se detalla un plan para el mantenimiento del sistema en su **Versión 2.0**.

**Mantenimiento Correctivo**
* **ID: MC-01:** Solucionar que las **notificaciones no funcionan en modo ahorro de energía**. Es de prioridad crítica y tiene un tiempo estimado de **2 semanas** con un costo de **$2,000 USD**.

**Mantenimiento Adaptativo**
* **ID: MA-01:** Implementar la **integración bidireccional con Google Calendar y Outlook**. Es de prioridad media y tiene un tiempo estimado de **4 semanas** con un costo de **$5,000 USD**.

**Mantenimiento Perfectivo**
* **ID: MP-01:** Agregar una nueva **vista de *timeline*** para visualización de citas. Es de prioridad baja y tiene un tiempo estimado de **3 semanas** con un costo de **$3,500 USD**.

El **Costo Total Estimado** es de **$10,500 USD** con un tiempo total de **9 semanas**. La recomendación es priorizar el mantenimiento Correctivo (MC-01) por ser crítico.

---

### 4. Investigación sobre Markdown

Markdown es un lenguaje de marcado ligero creado en 2004, cuyo objetivo es permitir que un documento en texto plano sea fácil de leer y convertir a HTML.

* **Uso en Software:** Se ha convertido en estándar para documentación (*README.md*, *LICENSE.md*), ya que permite escribir documentación de manera ágil.
* **Integración con Git:** Al ser texto plano, es ideal para el control de versiones (Git) ya que permite mostrar diferencias y resolver conflictos con precisión.
* **GitHub Flavored Markdown (GFM):** GitHub utiliza una variante que añade funciones como tablas, listas de tareas y referencias automáticas a *issues*.
