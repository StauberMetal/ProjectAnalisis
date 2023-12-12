Casos de Utilización para el Sistema de Registro de Asistencia con Tarjetas del Metro:


UC-001: Registro Automático de Asistencia:
Importancia: Primario
Actor: Usuario
Descripción: Registrar automáticamente la asistencia al presentar la tarjeta del metro.
Precondiciones: El usuario tiene una tarjeta del metro válida.
Flujo Principal:
Presentación de la tarjeta del metro al lector.
Verificación de la validez y registro de la entrada del usuario.
Confirmación visual o auditiva al usuario.
Flujos Alternativos:
Tarjeta Inválida: Mensaje de error si la tarjeta no es válida o está vencida.
Registro de Salida Automático: Al salir, la presentación de la tarjeta registra automáticamente la salida.
Postcondiciones:
Registro de la entrada del usuario.

UC-002: Consulta de Asistencia por Usuario:
Importancia: Primario
Actor: Administrador del Sistema
Descripción: Consultar la asistencia de un usuario en un rango de fechas.
Precondiciones: Inicio de sesión del administrador.
Flujo Principal:
Acceso a la sección de consulta de asistencia.
Selección del usuario y definición del rango de fechas.
Recuperación y visualización de la información detallada de la asistencia del usuario.
Flujos Alternativos:
Sin Asistencia Registrada: Informe si no hay registros para el usuario y período especificado.
Postcondiciones:
Información detallada de la asistencia del usuario mostrada.

UC-003: Configuración de Políticas de Asistencia:
Importancia: Primario
Actor: Administrador del Sistema
Descripción: Configurar políticas de asistencia, como horarios y días no laborables.
Precondiciones: Inicio de sesión del administrador.
Flujo Principal:
Acceso a la sección de configuración de políticas de asistencia.
Modificación de parámetros como horarios y días feriados.
Actualización en tiempo real de las políticas.
Flujos Alternativos:
Restricción de Acceso: Notificación si las nuevas políticas restringen el acceso a ciertos usuarios.
Postcondiciones:
Aplicación de las nuevas políticas de asistencia.

UC-004: Generación de Estadísticas de Asistencia:
Importancia: Secundario
Actor: Administrador del Sistema
Descripción: Generar estadísticas de asistencia para evaluar patrones y tendencias.
Precondiciones: Inicio de sesión del administrador en la interfaz de informes.
Flujo Principal:
Acceso a la sección de estadísticas de asistencia.
Selección de parámetros como período y usuarios específicos.
Generación de un informe estadístico mostrando patrones y tendencias de asistencia.
Flujos Alternativos:
Comparación de Grupos: Posibilidad de comparar la asistencia entre diferentes grupos de usuarios.
Postcondiciones:
Generación de estadísticas para análisis.

UC-005: Administración de Tarjetas Perdidas:
Importancia: Secundario
Actor: Administrador del Sistema
Descripción: Gestión de tarjetas perdidas y su impacto en la asistencia.
Precondiciones: Reporte de pérdida de una tarjeta del metro.
Flujo Principal:
Acceso a la interfaz de administración de tarjetas perdidas.
Registro de la tarjeta como no válida y notificación al usuario sobre la pérdida.
Ajuste en la base de datos para bloquear futuros registros con la tarjeta perdida.
Flujos Alternativos:
Desbloqueo de Tarjeta: Posibilidad de desbloquear la tarjeta si el usuario la encuentra.
Postcondiciones:
Tarjeta perdida registrada como no válida, evitando su uso futuro en el registro de asistencia. Usuario notificado con opción de desbloqueo.

UC-006: Generación de Alertas por Baja Asistencia:
Importancia: Secundario
Actor: Sistema
Descripción: Generar alertas ante una asistencia inusualmente baja.
Precondiciones: Sistema en funcionamiento y monitoreo de asistencia.
Flujo Principal:
Detección de baja asistencia en un período específico.
Generación de alerta visual o auditiva para notificar al administrador.
Flujos Alternativos:
Investigación de Causas: Acceso a informes detallados para investigar posibles causas de la baja asistencia.
Postcondiciones:
Administrador informado y posibilidad de tomar medidas.

UC-007: Desbloqueo de Tarjeta:
Importancia: Terciario
Actor: Usuario y Administrador del Sistema
Descripción: Desbloqueo de una tarjeta previamente bloqueada.
Precondiciones: Usuario presenta la tarjeta bloqueada al personal.
Flujo Principal:
Acceso a la interfaz de desbloqueo.
Selección de la opción para desbloquear una tarjeta.
Desbloqueo de la tarjeta para permitir futuros registros.
Flujos Alternativos:
Renovación de Tarjeta: Recomendación de renovar la tarjeta si ha pasado mucho tiempo desde el bloqueo.
Postcondiciones:
Tarjeta previamente bloqueada queda desbloqueada y puede usarse nuevamente.

UC-008: Registro Manual de Asistencia:
Importancia: Terciario
Actor: Administrador del Sistema
Descripción: Registro manual de la asistencia en situaciones excepcionales.
Precondiciones: Administrador ha iniciado sesión.
Flujo Principal:
Acceso a la interfaz de registro manual.
Ingreso de detalles, incluida la información de la tarjeta y la marca de tiempo.
Registro manual de la asistencia.
Flujos Alternativos:
Verificación de Identidad: Posibilidad de requerir verificación adicional antes de registrar la asistencia manualmente.
Postcondiciones:
Registro de la asistencia del usuario de manera manual en el sistema.

UC-009: Consulta de Estado de la Tarjeta:
Importancia: Terciario
Actor: Usuario
Descripción: Consulta del estado actual de la tarjeta del metro.
Precondiciones: Usuario accede a la interfaz de consulta.
Flujo Principal:
Ingreso a la sección de consulta de estado de la tarjeta.
Sistema muestra información sobre validez, historial y estado actual de la tarjeta.
Flujos Alternativos:
Bloqueo de Tarjeta: Instrucciones sobre cómo proceder si la tarjeta está bloqueada.
Postcondiciones:
Usuario obtiene información actualizada sobre el estado de su tarjeta del metro.

UC-010: Notificación de Mantenimiento del Sistema:
Importancia: Secundario
Actor: Administrador del Sistema
Descripción: Notificación a usuarios y administradores sobre mantenimiento programado.
Precondiciones: Sistema con período de mantenimiento programado.
Flujo Principal:

Acceso a la interfaz de programación de mantenimiento.
Definición de fechas y horas programadas.
Emisión de notificaciones automáticas a usuarios y administradores antes del inicio del mantenimiento.
Flujos Alternativos:
Cancelación de Mantenimiento: Posibilidad de cancelar o modificar el período de mantenimiento.
Postcondiciones:
Usuarios y administradores informados sobre mantenimiento programado, permitiendo una gestión eficiente de la asistencia durante esos intervalos.



