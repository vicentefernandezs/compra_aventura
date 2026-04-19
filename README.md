# 🛒 Comparador de Precios: Solución a la Asimetría de Información

## 📝 Problemática
Nuestro proyecto se enfoca en resolver la **asimetría de información** en el mercado de consumo masivo mediante un motor de búsqueda y comparación de precios. El objetivo principal es implementar una plataforma que permita a los usuarios visualizar comparativas de costos, ofertas vigentes y disponibilidad de stock en tiempo real entre distintas cadenas de supermercados, garantizando la **integridad de los datos** y optimizando la **eficiencia en la toma de decisiones**.

---

## 👥 Equipo de Trabajo (Scrum)

* **Product Owner:** René
* **Scrum Master:** Enano
* **Developers (Devs):**
    * Negra
    * Mole
    * Maski

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

Se ha optado por una **arquitectura multicapa distribuida** para asegurar escalabilidad:

* **Capa de Cliente (Frontend):** Interfaz responsiva comunicada mediante HTTP/REST (JSON).
* **Capa de Acceso (API Gateway):** Gestiona el Auth Service y un **Rate Limiter** para estabilidad.
* **Capa de Lógica (Backend):** Motor de búsqueda, lógica de ordenamiento y validador de stock.
* **Capa de Integración (Adaptadores):** Conectores específicos para **Lider, Jumbo y Santa Isabel**.
* **Capa de Datos (Persistencia):** * **PostgreSQL/MySQL:** Datos de usuarios.
    * **Redis:** Cacheo temporal de precios para máximo rendimiento.

---

## 🛡️ Atributos de Calidad

* **SEGURIDAD (Prioridad Alta):** Autenticación centralizada y cifrado de extremo a extremo.
* **USABILIDAD:** Diseño centrado en el usuario para reducir el esfuerzo mental.
* **DISPONIBILIDAD:** Datos precisos y consistentes sobre el stock por supermercado.
* **RENDIMIENTO:** Latencia mínima mediante optimización de consultas y uso de caché.

---

## 🎨 Diseño (Figma)
Puedes revisar el prototipo funcional en el siguiente enlace:
🔗 [Prototipo en Figma](https://rack-studio-58141370.figma.site/login)
