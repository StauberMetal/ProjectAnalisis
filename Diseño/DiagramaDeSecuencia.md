@startuml

actor Profesor
actor Administrador 
boundary SistemaDeAsistencia
database BaseDeDatos 

activate Profesor
activate App
activate BaseDeDatos

group Registro Automático de Asistencia

Profesor -> App: Inicia Sesión

Profesor -> App: Selecciona "Registro de Asistencia"
App -> App: Muestra interfaz de registro
Profesor -> App: Utiliza lector NFC

App -> BaseDeDatos: Consulta información del estudiante
BaseDeDatos --> App: Devuelve detalles del estudiante
App -> BaseDeDatos: Registra asistencia

BaseDeDatos --> App: Confirmación de registro
App --> Profesor: Confirmación visual/auditiva
end

group Administración de Grupos

opt Profesor 
Profesor -> App: Inicia Sesión

Profesor -> App: Selecciona "Administración de Grupos"
App -> App: Muestra interfaz de administración de grupos
Profesor -> App: Realiza ajustes en la composición de grupos

App -> BaseDeDatos: Actualiza información de composición de grupos
BaseDeDatos --> App: Confirmación de actualización
App --> Profesor: Confirmación visual/auditiva

else Administrador 
activate Administrador 

Administrador -> App: Inicia Sesión

Administrador -> App: Selecciona "Administración de Grupos"
App -> App: Muestra interfaz de administración de grupos
Administrador -> App: Realiza ajustes en la composición de grupos

App -> BaseDeDatos: Actualiza información de composición de grupos
BaseDeDatos --> App: Confirmación de actualización
App --> Administrador : Confirmación visual/auditiva
end 
deactivate Administrador

end

group Administración de Alumnos

opt Profesor 
Profesor -> App: Inicia Sesión

Profesor -> App: Selecciona "Administración de Alumnos"
App -> App: Muestra interfaz de administración de alumnos
Profesor -> App: Realiza cambios en los detalles de los estudiantes

App -> BaseDeDatos: Actualiza información de detalles de estudiantes
BaseDeDatos --> App: Confirmación de actualización
App --> Profesor: Confirmación visual/auditiva

else Administrador 
activate Administrador
Administrador-> App: Inicia Sesión

Administrador-> App: Selecciona "Administración de Alumnos"
App -> App: Muestra interfaz de administración de alumnos
Administrador-> App: Realiza cambios en los detalles de los estudiantes

App -> BaseDeDatos: Actualiza información de detalles de estudiantes
BaseDeDatos --> App: Confirmación de actualización
App --> Administrador: Confirmación visual/auditiva
end
deactivate Administrador
end 

group Consulta de Asistencia por Profesor
Profesor -> App: Inicia Sesión

Profesor -> App: Selecciona "Consulta de Asistencia"
App -> App: Muestra interfaz de consulta
Profesor -> App: Selecciona rango de fechas y grupos

App -> BaseDeDatos: Consulta asistencia por parámetros
BaseDeDatos --> App: Devuelve información de asistencia
App --> Profesor: Muestra información detallada
end


deactivate Profesor
deactivate App
deactivate BaseDeDatos


@enduml
