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
| **Máximo Torrijo Espinoza** | Developer | Capa de Cliente (Frontend), Módulo de Autenticación (JWT), Diseño de Interfaz (Figma. |
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
    * **Redis:** Cacheo temporal de precios para optimizar el rendimiento y minimizar la latencia de respuesta.

---

## 💻 Stack Tecnológico (Gestión del Sistema)

De acuerdo a la arquitectura distribuida, el sistema es gestionado bajo el siguiente esquema de responsabilidades técnicas:

* **Capa de Cliente:** Maneja la interfaz responsiva y la comunicación asíncrona mediante JSON.
* **Capa de Acceso:** Gestiona la seguridad centralizada (Auth Service) y el control de tráfico (Rate Limiter).
* **Capa de Lógica:** Maneja el motor de búsqueda, las reglas de comparación y la integridad de los datos de stock.
* **Capa de Integración:** Gestiona los adaptadores que permiten la interoperabilidad con fuentes externas (Lider, Jumbo, Santa Isabel).
* **Capa de Datos:** Maneja la persistencia de usuarios en BD relacionales y la velocidad de respuesta mediante el cacheo en Redis.

---


---

## ⚙️ Características Funcionales

| Módulo | Descripción |
| :--- | :--- |
| **Autenticación** | Sistema centralizado con credenciales cifradas mediante **JWT**. |
| **Comparativa Multitienda** | Despliegue de precios y ofertas de diversas fuentes simultáneamente. |
| **Sugerencias Dinámicas** | Motor de recomendaciones para minimizar la carga cognitiva. |
| **Monitoreo de Stock Real** | Verificación de disponibilidad de artículos en tiempo real. |
| **Dashboard de Ofertas** | Panel principal con artículos destacados por relevancia. |

---

## 🎨 Diseño (Figma)
Puedes revisar el prototipo funcional en el siguiente enlace:
🔗 [Prototipo en Figma](https://rack-studio-58141370.figma.site/login)
