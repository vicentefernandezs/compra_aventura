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
| **US-01** | Registrar cuenta de usuario | #12 |
| **US-02** | Iniciar sesión | #13 |
| **US-03** | Búsqueda de productos por filtros | #14 |
| **US-04** | Comparación de precios multitienda | #15 |
| **US-05** | Visualización de disponibilidad de stock | #16 |
| **US-06** | Dashboard de ofertas destacadas | #17 |



---

## 🧩 Entidades de Dominio

El sistema se compone de las siguientes entidades principales (objetos del mundo real):

* **Usuario**
    - id, nombre, email, contraseña
* **Producto**
    - id, nombre, categoría
* **Supermercado**
    - id, nombre, ubicación
* **Precio**
    - id, valor, fecha, producto_id, supermercado_id
* **Oferta**
    - id, descuento, vigencia

> **Nota:** El "Comparador" se implementa como un servicio de lógica de sistema y no como una entidad de dominio.

---


## ⚙️ Características Funcionales

| Módulo | Descripción |
| :--- | :--- |
| **Autenticación** | Sistema centralizado con credenciales cifradas mediante **JWT**. |
| **Comparativa Multitienda** | Despliegue de precios y ofertas de diversas fuentes simultáneamente. |
| **Sugerencias Dinámicas** | Motor de recomendaciones para minimizar la carga cognitiva. |
| **Monitoreo de Stock Real** | Verificación de disponibilidad de artículos en tiempo real. |

---

## 🎨 Diseño (Figma)
🔗 [Prototipo en Figma](https://rack-studio-58141370.figma.site/login)
