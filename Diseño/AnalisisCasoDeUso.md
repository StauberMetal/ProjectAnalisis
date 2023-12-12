Análisis de Caso de Uso para el Sistema de Asistencia para Profesores de FCA en Android/iOS:

UC-001: Registro Automático de Asistencia (Primario):

Tipo: Proceso Transaccional

Usuario: Profesor.

Descripción: La aplicación captura automáticamente la presencia de los estudiantes mediante el escaneo de tarjetas de metro usando la tecnología NFC. Antes de iniciar, se requiere que el profesor haya iniciado sesión en la aplicación.

Flujo Principal:

1. El profesor selecciona la opción "Registro de Asistencia".

2. Utiliza el lector NFC del dispositivo para escanear las tarjetas de metro de los estudiantes.

3. La aplicación verifica la validez de las tarjetas y registra la asistencia en tiempo real.

4. Se proporciona una confirmación visual o auditiva para informar al profesor sobre el éxito del registro.

Subflujo - Notificación de Cambios en la Asistencia (Secundario):

a. Se detectan alteraciones sustanciales en la asistencia.

b. Se generan notificaciones automáticas para informar a los profesores afectados.

c. Los profesores reciben información sobre los cambios en tiempo real.

Subflujo - Gestión de Errores de Tarjeta (Secundario):

a. Durante el proceso de registro de asistencia, se identifican tarjetas inválidas o problemas de lectura.

b. Se generan mensajes de error o notificaciones para informar al profesor.

c. La asistencia se registra con éxito solo después de resolver los problemas.


UC-002: Administración de Grupos (Primario):

Tipo: Proceso Administrativo

Usuario: Profesor o Administrador.

Descripción: Este proceso permite realizar cambios en la composición de grupos, como altas, bajas o modificaciones en los estudiantes. La condición previa es que el profesor o el administrador haya iniciado sesión en la aplicación.

Flujo Principal:

1. El Profesor/Administrador accede a la sección "Administración de Grupos".

2. Realiza los ajustes necesarios en la composición de los grupos de estudiantes.

3. Se confirma y actualiza inmediatamente la información.

Subflujo - Notificación de Cambios en la Composición de Grupos (Secundario):

a. Se detectan cambios en la composición de grupos.

b. Se generan notificaciones automáticas para informar a los profesores afectados.

c. Los profesores son informados sobre los cambios en tiempo real.

UC-003: Administración de Alumnos (Primario):

Tipo: Proceso Administrativo
Usuario: Profesor o Administrador.
Descripción: Este proceso permite realizar cambios en la información de los estudiantes, incluyendo altas, bajas o modificaciones. La condición previa es que el profesor o el administrador haya iniciado sesión en la aplicación.
Flujo Principal:
Profesor/Administrador accede a la sección de "Administración de Alumnos".
Realiza los cambios necesarios en los detalles de los estudiantes.
Se confirma y actualiza inmediatamente la información.


UC-004: Administración de Tarjetas (Primario):

Tipo: Proceso Administrativo
Usuario: Profesor o Administrador.
Descripción: Este proceso permite realizar ajustes en la información asociada a las tarjetas de metro de los estudiantes, como altas, bajas o modificaciones. La condición previa es que el profesor o el administrador haya iniciado sesión en la aplicación.
Flujo Principal:

Profesor/Administrador accede a la sección de "Administración de Tarjetas".
Realiza los ajustes necesarios en la información de las tarjetas.
Se confirma y actualiza inmediatamente la información.

UC-005: Consulta de Asistencia por Profesor (Primario):
Tipo: Proceso de Consulta
Usuario: Profesor.
Descripción: Permite al profesor revisar el historial de asistencia de estudiantes en un período específico. La condición previa es que el profesor haya iniciado sesión en la aplicación.
Flujo Principal:
El profesor accede a la sección de "Consulta de Asistencia".
Selecciona el rango de fechas y los grupos de estudiantes de interés.
Visualiza la información detallada de la asistencia de los estudiantes.

UC-006: Notificación de Cambios en la Asistencia (Secundario):
Tipo: Notificación
Usuario: Sistema.
Descripción: Envía alertas automáticas a profesores sobre cambios significativos en la asistencia. La condición previa es que el sistema esté operativo.
Flujo Principal:
Detección de alteraciones sustanciales en la asistencia.
Generación de notificaciones automáticas para informar a los profesores afectados.
Profesores son informados de los cambios en tiempo real.

UC-007: Gestión de Errores de Tarjeta (Secundario):
Tipo: Notificación
Usuario: Profesor.
Descripción: Recibir mensajes de error o notificaciones en caso de problemas con las tarjetas del metro durante el registro de asistencia. La condición previa es que el profesor haya iniciado sesión.
Flujo Principal:
Durante el proceso de registro de asistencia, identificación de tarjetas inválidas o problemas de lectura.
Generación de mensajes de error o notificaciones para informar al profesor.
La asistencia se registra con éxito solo después de resolver los problemas.

UC-008: Notificación de Cambios en la Composición de Grupos (Secundario):
Tipo: Notificación
Usuario: Sistema.
Descripción: Enviar notificaciones automáticas a profesores sobre modificaciones en la composición de grupos. La condición previa es que el sistema esté operativo.
Flujo Principal:
Detección de cambios en la composición de grupos.
Generación de notificaciones automáticas a los profesores afectados.
Profesores son informados de los cambios en tiempo real.


UC-009: Generación de Reportes de Asistencia (Secundario):
Tipo: Proceso de Consulta
Usuario: Administrador.
Descripción: Crear informes detallados de la asistencia para análisis y seguimiento. La condición previa es que el administrador haya iniciado sesión.
Flujo Principal:
El administrador accede a la sección de "Generación de Reportes".
Define parámetros como el período y los grupos de interés.
La aplicación genera un informe detallado de la asistencia.
Visualización y descarga del informe por parte del administrador.


UC-010: Administración de Cambios en la Información de Alumnos (Secundario):
Tipo: Proceso de Consulta
Usuario: Administrador.
Descripción: Seguir los cambios recientes en la información de los estudiantes. La condición previa es que el administrador haya iniciado sesión.
Flujo Principal:
El administrador accede a la sección de "Historial de Cambios".
Visualiza los cambios recientes en la información de los estudiantes.
Posibilidad de revertir cambios si es necesario.

UC-011: Configuración de Notificaciones (Secundario):
Tipo: Configuración
Usuario: Profesor o Administrador.
Descripción: Personalizar las preferencias de notificación para eventos específicos, como cambios en grupos o errores de tarjetas. La condición previa es que el profesor o el administrador haya iniciado sesión.
Flujo Principal:
Acceso a la sección de "Configuración de Notificaciones".
Definición de preferencias de notificación para eventos específicos.
Confirmación y aplicación de las configuraciones.


UC-012: Registro de Informes por Periodo de Tiempo (Primario):

Tipo: Proceso de Consulta
Usuario: Administrador.
Descripción: Permite al administrador registrar informes específicos durante un período de tiempo definido para su posterior consulta y análisis. La condición previa es que el administrador haya iniciado sesión en la aplicación.
Flujo Principal:

El administrador accede a la sección de "Registro de Informes por Periodo de Tiempo".
Selecciona el rango de fechas para el cual desea generar el informe.
Define otros parámetros relevantes, como grupos específicos si es necesario.
La aplicación genera un informe detallado durante el período especificado.
Visualización y descarga del informe por parte del administrador.
UC-013: Exportar Informe (Primario):
Tipo: Proceso de Exportación
Usuario: Administrador.
Descripción: Permite al administrador exportar informes generados para su almacenamiento o uso externo. La condición previa es que el administrador haya iniciado sesión en la aplicación y haya generado un informe previamente.
Flujo Principal:
El administrador accede a la sección de "Exportar Informe".
Selecciona el informe que desea exportar de la lista de informes disponibles.
Elige el formato de exportación deseado, como PDF o CSV.
La aplicación genera y proporciona un enlace de descarga para el informe exportado.
El administrador descarga el informe en el formato seleccionado.
Subflujo - Notificación de Exportación Exitosa (Secundario):
a. Después de descargar el informe, la aplicación envía una notificación al administrador confirmando la exportación exitosa.
b. El administrador recibe la notificación y verifica la exportación exitosa del informe.
