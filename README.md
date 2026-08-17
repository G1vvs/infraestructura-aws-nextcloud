# infraestructura-aws-nextcloud
# Plataforma de Gestión Documental Cloud en AWS

## 📌 Resumen del Proyecto
Diseño e implementación de una infraestructura cloud en AWS para centralizar la documentación corporativa de una empresa de obras civiles con operaciones en múltiples localidades. 

Este proyecto fue desarrollado en equipo para pasar de la teoría y los diagramas a un despliegue real en la nube, resolviendo un problema de negocio concreto.

## ⚠️ El Problema
La empresa operaba con documentación crítica dispersa entre distintas faenas, carpetas locales y correos electrónicos (contratos, permisos, registros laborales). Existía una falta total de un sistema común, lo que generaba:
- Riesgo legal por pérdida de información.
- Ausencia de respaldos automatizados.
- Nulo control de acceso unificado.

## 🚀 La Solución Arquitectónica
Se diseñó y desplegó una infraestructura cloud real que centralizó las operaciones mediante contenedores.

**Stack Tecnológico:** AWS (EC2, S3, RDS), Docker, Nextcloud, Nginx, PostgreSQL, OpenLDAP, Redis, Debian.

### Componentes del Despliegue:
* **Cómputo:** 6 instancias Amazon EC2 ejecutando servicios contenerizados con Docker sobre Debian (Nextcloud, Nginx, OpenLDAP, Redis).
* **Almacenamiento:** Centralización de archivos y respaldos utilizando Amazon S3.
* **Base de Datos:** PostgreSQL configurado sobre Amazon RDS Multi-AZ para garantizar alta disponibilidad.
* **Seguridad y Acceso:** Autenticación de usuarios y control de accesos centralizado mediante OpenLDAP integrado a Nextcloud.

## 📸 Evidencia del Despliegue

**1. Infraestructura de Cómputo (AWS EC2)**
*Panel de administración mostrando las instancias de Nextcloud, OpenLDAP, Nginx y Redis en ejecución.*
![Instancias EC2](./assets/image_5a31c6.jpg)

**2. Almacenamiento Centralizado (AWS S3)**
*Configuración del bucket para el respaldo seguro de la documentación.*
![Bucket S3](./assets/image_5a31ac.png)

**3. Autenticación Integrada**
*Interfaz de acceso seguro al sistema.*
<img width="1280" height="610" alt="1781311165254" src="https://github.com/user-attachments/assets/d5e23a31-d73d-4baa-879b-e001ab3d1f1e" />

**4. Interfaz de Usuario Final**
*Dashboard operativo de la plataforma desplegada.*
![Dashboard Nextcloud](./assets/image_5a31a6.jpg)

## 💡 Aprendizajes Clave
Más allá del stack tecnológico, el mayor valor de este proyecto fue la ejecución práctica: verificar la comunicación entre instancias, configurar el almacenamiento en S3 y validar la autenticación en red. Fue un primer paso concreto en infraestructura cloud, demostrando la capacidad de proponer una solución a un problema real y desplegarla con éxito.


