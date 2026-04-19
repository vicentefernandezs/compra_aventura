# 🛒 Compra Aventura: Sistema Inteligente de Comparativa Multitienda y Optimización de Consumo

## 📝 Problemática
Nuestro proyecto aborda la falta de transparencia en el mercado de consumo masivo mediante un motor de búsqueda avanzado. El objetivo es eliminar la brecha de información entre las cadenas de retail y los consumidores, permitiendo comparar costos, ofertas y disponibilidad de stock en tiempo real para facilitar una toma de decisiones eficiente y segura.

---

## 👥 Equipo de Trabajo (Scrum)

* **Scrum Master:** Vicente Fernandez Simonetti
* **Product Owner:** Joaquín Rodríguez López
* **Developers (Devs):**
    * Máximo Torrijo Espinoza
    * Joaquín Thomas Rojas Toledo

---

## 🛠️ Responsabilidades del Equipo

| Integrante | Rol | Ítems de la rúbrica a cargo |
| :--- | :--- | :--- |
| **Vicente Fernandez Simonetti** | Scrum Master | Facilitación de Ceremonias, Gestión de Impedimentos, Seguimiento de Atributos de Calidad. |
| **Joaquín Rodríguez López** | Product Owner | Gestión de Backlog, Definición de Historias de Usuario (US), Validación de Valor de Negocio. |
| **Máximo Torrijo Espinoza** | Developer | Capa de Cliente (Frontend), Módulo de Autenticación (JWT), Diseño de Interfaz (Figma). |
| **Joaquín Thomas Rojas Toledo** | Developer | Capa de Lógica (Backend), Integración de Adaptadores (APIs Externas), Persistencia (SQL/Redis). |

---

## 📋 Historias de Usuario (Backlog)

| ID | Nombre | Issue |
| :--- | :--- | :--- |
| **US-01** | Registrar cuenta de usuario | #1 |
| **US-02** | Iniciar sesión (Auth JWT) | #2 |
| **US-03** | Búsqueda de productos por filtros | #3 |
| **US-04** | Comparación de precios multitienda | #4 |
| **US-05** | Visualización de disponibilidad de stock | #5 |
| **US-06** | Dashboard de ofertas destacadas | #6 |

---

## 📐 Diseño Arquitectónico

Se ha optado por una **arquitectura multicapa distribuida** para asegurar la escalabilidad, el mantenimiento y la correcta separación de responsabilidades:

* **Capa de Cliente (Frontend):** Interfaz responsiva diseñada para el usuario final que se comunica con el servidor mediante **HTTP/REST (JSON)**.
* **Capa de Acceso y Seguridad (API Gateway):** Gestiona el **Auth Service (JWT/Login)** y un **Rate Limiter** para evitar la saturación del sistema y garantizar un acceso seguro.
* **Capa de Lógica de Negocio (Backend):** Contiene el motor de búsqueda, la lógica de ordenamiento del comparador de precios y el validador de stock.
* **Capa de Integración (Adaptadores):** Implementa conectores específicos para cada cadena (**Lider, Jumbo, Santa Isabel**), permitiendo la interoperabilidad y el consumo de datos externos.
* **Capa de Datos (Persistencia):**
    * **Bases de Datos Relacionales (PostgreSQL/MySQL):** Para la gestión persistente de usuarios.
    * **Redis:** Cacheo temporal de precios para optimizar el rendimiento y minimizar la latencia.

---

## 🛡️ Atributos de Calidad (Requisitos Extrafuncionales)

El sistema debe cumplir con los siguientes estándares técnicos para asegurar una operación profesional:

* **Rendimiento:**
    * El sistema debe responder en menos de **2 segundos**.
    * Capacidad para soportar al menos **1000 usuarios simultáneos**.
* **Seguridad:**
    * Las contraseñas deben almacenarse encriptadas mediante algoritmos de hash seguros.
    * Implementación obligatoria de autenticación mediante **JWT (JSON Web Tokens)**.
* **Usabilidad:**
    * Interfaz intuitiva diseñada para minimizar la carga cognitiva.
    * Diseño **Responsivo** (accesible desde dispositivos móviles y escritorio).
* **Disponibilidad:**
    * Garantía de operatividad del **99%** del tiempo.
* **Compatibilidad:**
    * Soporte completo para navegadores **Chrome, Edge y Firefox**.
* **Escalabilidad:**
    * Arquitectura modular que permite aumentar la capacidad de procesamiento sin degradar el servicio.
* **Mantenibilidad:**
    * Código fuente documentado y organizado bajo estándares de limpieza.

---

## ⚙️ Características Funcionales

| Módulo | Descripción |
| :--- | :--- |
| **Módulo de Autenticación** | Manejo de sesiones y protección de credenciales cifradas. |
| **Comparativa Multitienda** | Despliegue simultáneo de precios y ofertas de diversas fuentes. |
| **Sugerencias Dinámicas** | Motor de recomendaciones para agilizar la búsqueda del usuario. |
| **Monitoreo de Stock Real** | Sincronización con góndolas virtuales para reflejar la realidad del mercado. |
| **Dashboard de Ofertas** | Panel de control con artículos destacados por relevancia. |

---

## 🎨 Diseño (Figma)
Puedes revisar el prototipo funcional y los diagramas visuales en el siguiente enlace:
🔗 [Prototipo en Figma](https://rack-studio-58141370.figma.site/login)
