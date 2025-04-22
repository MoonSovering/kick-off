# 🚀 Kick Off - Sistema de Reconocimiento de Objetos Perdidos con IA  
**Universidad:** Universidad de Cundinamarca  
**Fecha:** [16/04/2025]  
**Equipo:** Liam Software.  

---

## 🎯 Objetivo de la reunion
- Presentar el proyecto de IA para gestión de objetos perdidos.  
- Alinear expectativas con stakeholders (administración, seguridad, TI).  
- Definir cronograma y responsabilidades.  

---

## 1️⃣ Introducción  
**Contexto:**  
- Pérdida frecuente de objetos personales en campus (mochilas, celulares, llaves).  
- Falta de un sistema centralizado para reporte y recuperación.  

**Objetivo del Proyecto:**  
> "Desarrollar un sistema de IA que **automatice la identificación de objetos perdidos** mediante análisis de imágenes capturadas en el campus, vinculando reportes con dueños potenciales."  

---

## 2️⃣ Alcance del Proyecto  
| **Incluye**                                   | **No Incluye**                     |  
|-----------------------------------------------|------------------------------------|  
| Captura de imágenes en zonas comunes          | Reconocimiento facial              |  
| Base de datos de objetos reportados           | Reemplazo de personal de seguridad |  
| Notificaciones a dueños vía correo/APP        | Hardware de cámaras (solo software)|  

---

## 3️⃣ Stakeholders Clave  
| **Rol**                | **Responsable**      | **Contribución**                          |  
|------------------------|----------------------|-------------------------------------------|  
| Sponsor                | [Rectoría]           | Aprobación de presupuesto                 |  
| Equipo de Seguridad    | [Jefe de Seguridad]  | Validación de zonas de monitoreo          |  
| Departamento de TI     | [CIO]                | Infraestructura y integraciones           |  

---

## 4️⃣ Funcionamiento Técnico (Flujo)  
```mermaid
flowchart TD
    A[Cámaras capturan imágenes] --> B(IA analiza y clasifica objetos)
    B --> C{Objeto reportado como perdido?}
    C -->|Sí| D[Busca coincidencias en BD]
    C -->|No| E[Descarta imagen en X días]
    D --> F[Notifica al dueño vía email/APP]