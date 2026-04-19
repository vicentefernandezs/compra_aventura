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

## ## Responsabilidades del equipo

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

## 🚀 Requisitos Extrafuncionales

### 1. Rendimiento
- El sistema debe responder en menos de 2 segundos.
- Debe soportar al menos 1000 usuarios simultáneos.

### 2. Seguridad
- Las contraseñas deben almacenarse encriptadas.
- El sistema debe usar autenticación segura (**JWT**).

### 3. Usabilidad
- La interfaz debe ser intuitiva y fácil de usar.
- El sistema debe ser accesible desde dispositivos móviles.

### 4. Disponibilidad
- El sistema debe estar disponible el 99% del tiempo.

### 5. Compatibilidad
- Debe funcionar en navegadores Chrome, Edge y Firefox.

### 6. Escalabilidad
- El sistema debe poder aumentar su capacidad sin afectar el rendimiento.

### 7. Mantenibilidad
- El código debe estar documentado y organizado.

---

## 🔄 Flujo del Usuario

1.  **Autenticación:** El usuario accede mediante un login seguro para personalizar su experiencia.
2.  **Dashboard Principal:** Visualización de artículos destacados y ofertas relevantes.
3.  **Búsqueda y Filtro:** Selección de un artículo y procesamiento de la comparación multitienda.
4.  **Visualización de Resultados:** Presentación de precios, desglose de ofertas y verificación de stock.

---


---

## 🎨 Diseño (Figma)
Puedes revisar el prototipo funcional en el siguiente enlace:
🔗 [Prototipo en Figma](https://rack-studio-58141370.figma.site/login)
