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

* Registrar nuevos usuarios
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

# 5. Reglas de negocio

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

# 8. Requisitos no funcionales 

# 9. Plazos establecidos 

# 10. Alcanze y Presupuesto

# 11. Propuesta y Forma de Trabajo

# 12. 

# 13. Soporte y Mantenimiento

# 14. Tiempos de Reuniones y Proximos pasos 

# . Futuras Versiones (Excluye del MVP)

## Versión 2.0:

* **Notificaciones push y recordatorios**.
* **Reportes avanzados y analytics** (métricas de uso, ocupación, ingresos).
* Sistema de **reserva de equipos** específicos.
* **Planes de entrenamiento personalizados** (asignados por el staff/entrenador).
# Versión 3.0: 

## Sistema de logros y gamificación 
* **Chat interno con entrenadores** 
* **Control de progreso físico**