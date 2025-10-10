# Guía de Requerimientos - Sistema de Gestión para Gimnasio (Base de Datos NoSQL)

# 1. Descripción del Cliente y Problema Principal

Cliente: Gimnasio que enfrenta problemas de gestión operativa
Problema Principal: Sistema ineficiente que genera:

* Mala gestión de usuarios y membresías
* Problemas con control de horarios y aforo
* Poca administración y seguimiento de ingresos
* Falta de control en el acceso al establecimiento

---

# 2. Tipos de Usuarios y Perfiles con Permisos

## Administrador (Dueño)

**Permisos**:

* Gestión completa de usuarios (crear, editar, eliminar)
* Administración de membresías y planes
* Gestión de trabajadores
* Reportes y estadísticas
* Configuración del sistema
* Control de horarios y aforo

## Trabajadores (Staff)

**Permisos**:

* Verificar estado de membresías
* Asistir a clientes en el gimnasio
* Consultar horarios y disponibilidad
* Reportar incidencias

## Clientes

**Sub-roles**:

* Estudiantes
* Profesores

**Permisos**:

* Registrarse en el sistema
* Agendar y des agendar horarios
* Ver su historial de ingresos
* Gestionar su perfil
* Eliminar su cuenta
* Ver estado de su membresía

---

# 3. Definición del MVP (Minimum Viable Product)

## MVP - Versión 1.0 (Incluye)

### Funcionalidades Core:

* **Registro de usuarios** con datos básicos (actualizable con huella digital).
* Sistema de **autenticación por huella digital** en pórtico.
* **Gestión de membresías** (estados: activa, expirada, suspendida).
* **Agendamiento básico** de horarios por piso.
* **Control de acceso** basado en membresía activa.
* **Bloqueo/permiso de acceso** desde aplicación.

### Características Técnicas:

* Base de datos **NoSQL (MongoDB)**.
* **Aplicación web** para administración.

# 4. Datos que se necesitan Guardar
* Datos de clientes  
* Membresia
* Hora agendada
* Entrada y salida por huella   

# 5. Reglas de negocio
* El desajendamiento de hora actualizara automaticamente el stock de horas disponibles
* El agendamiento de hora solo se puede hacer con una hora de anticipación.
# 6.  Prioridades de Desarrollo

### Alta Prioridad
* **Sistema de autentificación por huella**
* **Gestion de estado de membresía**
* **Registro de ingresos/salidas**
* **Agendamiento de horario**

### Media Prioridad
* **Dashboard administrativo**
* **Control básico de acceso**

### Baja Prioridad
* **Reportes avanzados**
* **Integraciones adicionales**

# 7. Flujos Principales
* 1.Flujo de Autentificacion 
* Registro de Usuario:

    1. El usuario presiona "Registrarse"
    2. Ingresa Datos (Nombre, rut, email, contraseña)
    3. Acepta términos y condiciones
    4. Acceder a la pantalla principal
* Inicio de Sesión (Login):

    1. El usuario accede a la pantalla de login.
    2. Ingresa sus credenciales (email y contraseña).
    3. Presiona "Iniciar Sesión".
    4. Si es correcto, accede a la pantalla principal.
    5. Flujo Alternativo: Si las credenciales son incorrectas, se muestra un mensaje de error.
* 2.Flujo de Gestión de agendas
*   Reserva de gimnasio:
    1. El usuario navega a la seleccion de "Agendar"
    2. Selecciona los dias y horas disponibles
    3. Confirma Reserva
    4. Se le agrega en la pantalla principal
*   Cancelacion de reserva:
    1. El usuario accede a la pantalla principal
    2. Selecciona la reserva que desea cancelar 
    3. Confirma la cancelacion
    4. La Reserva se libera y el usuario recibe una notificacion
* 3.Flujo de Gestion de Membresía
*   Informacion membresia:
    1. El usuario accede a la seccion de "Membresia"
    2. Visualiza el estado de su membresia
# 8. Requisitos no funcionales 
* Seguridad de los datos de los usuarios 
# 9. Plazos establecidos 
* Entrega de requisitos 21/10
* Primer prototipo ?/11
* Entre de mvp funcional ?/12 
# 10. Alcanze y Presupuesto
* Municipalidades de comunas/Gimnacios 
# 11. Propuesta y Forma de Trabajo

# 12. Soporte y Mantenimiento
* Se dara 3 meses de soporte despues de la entrega del proyecto 

# 13. Tiempos de Reuniones y Proximos pasos
* Reuniones cada semana para ver el avanze del proyecto   

# Futuras Versiones (Excluye del MVP)

## Versión 2.0:

* **Notificaciones push y recordatorios**.
* **Reportes avanzados y analytics** (métricas de uso, ocupación, ingresos).
* Sistema de **reserva de equipos** específicos.
* **Planes de entrenamiento personalizados** (asignados por el staff/entrenador).

## Versión 3.0: 

### Sistema de logros y gamificación 
* **Chat interno con entrenadores** 
* **Control de progreso físico**
