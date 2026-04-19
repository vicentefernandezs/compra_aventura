# 🛒 SmartPrice: Sistema Inteligente de Comparativa Multitienda y Optimización de Consumo

## 📝 Problemática
Nuestro proyecto aborda la falta de transparencia en el mercado de consumo masivo mediante un motor de búsqueda avanzado. El objetivo es eliminar la brecha de información entre las cadenas de retail y los consumidores, permitiendo comparar costos, ofertas y disponibilidad de stock en tiempo real para facilitar una toma de decisiones eficiente y segura.

---

## 👥 Equipo de Trabajo (Scrum)

* **Product Owner:** Joaquín Rodríguez López
* **Scrum Master:** Vicente Fernandez Simonetti
* **Developers (Devs):**
    * Máximo Torrijo Espinoza
    * Joaquín Thomas Rojas Toledo

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

## ⚙️ Características Funcionales

| Módulo | Descripción |
| :--- | :--- |
| **Autenticación** | Sistema centralizado con manejo de sesiones y credenciales cifradas mediante **JWT**. |
| **Comparativa Multitienda** | Motor de procesamiento que despliega precios y ofertas de diversas fuentes simultáneamente. |
| **Sugerencias Dinámicas** | Interfaz intuitiva con recomendaciones para minimizar la carga cognitiva. |
| **Monitoreo de Stock** | Verificación en tiempo real para asegurar que la consulta refleje la realidad de las góndolas. |
| **Filtros Avanzados** | Procesamiento de comparación inmediata por categorías y artículos generales. |
| **Dashboard de Ofertas** | Panel principal con artículos destacados basados en algoritmos de relevancia. |
| **Optimización de Latencia** | Consultas optimizadas para el despliegue rápido desde múltiples fuentes externas. |

---

## 🔄 Flujo del Usuario

1.  **Autenticación:** El usuario accede mediante un login seguro para personalizar su experiencia.
2.  **Dashboard Principal:** Visualización de artículos destacados y ofertas relevantes.
3.  **Búsqueda y Filtro:** Selección de un artículo y procesamiento de la comparación multitienda.
4.  **Visualización de Resultados:** Presentación de precios, desglose de ofertas y verificación de stock.

---

## 🏗️ Arquitectura del Sistema

Se ha optado por una **arquitectura multicapa distribuida** para asegurar escalabilidad y separación de responsabilidades:

* **Capa de Cliente (Frontend):** Interfaz responsiva comunicada mediante HTTP/REST (JSON).
* **Capa de Acceso (API Gateway):** Gestiona el Auth Service y un **Rate Limiter** para estabilidad.
* **Capa de Lógica (Backend):** Motor de búsqueda, lógica de ordenamiento y validador de stock.
* **Capa de Integración (Adaptadores):** Conectores específicos para la interoperabilidad con **Lider, Jumbo y Santa Isabel**.
* **Capa de Datos (Persistencia):**
    * **PostgreSQL / MySQL:** Para gestión de usuarios y datos relacionales.
    * **Redis:** Cacheo temporal de precios para optimizar el rendimiento.

---

## 🛡️ Atributos de Calidad

* **SEGURIDAD (Prioridad Alta):** Autenticación centralizada y manejo de credenciales cifradas.
* **USABILIDAD:** Interfaz diseñada para minimizar la carga cognitiva mediante sugerencias dinámicas.
* **DISPONIBILIDAD:** Entrega de datos precisos sobre el stock para reflejar la realidad del mercado.
* **RENDIMIENTO:** Optimización de consultas y uso de caché para latencia mínima.

---

## 🎨 Diseño (Figma)
Puedes revisar el prototipo funcional en el siguiente enlace:
🔗 [Prototipo en Figma](https://rack-studio-58141370.figma.site/login)
