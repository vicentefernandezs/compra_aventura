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



## 🧩 Entidades del Dominio

El sistema se articula en torno a las siguientes entidades que gestionan la lógica del negocio:

* **Usuario:** Maneja el perfil personal, las credenciales de acceso y las preferencias de búsqueda dentro de la plataforma.
* **Producto:** Maneja la información técnica, categorías y descriptores de los artículos consultados.
* **Tienda:** Maneja la relación con los proveedores externos, incluyendo la ubicación de sucursales y la disponibilidad de servicios.
* **Comparador:** Maneja el núcleo de la lógica; procesa precios, ofertas vigentes y niveles de stock de múltiples fuentes en tiempo real.

---



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
