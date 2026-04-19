================================================================================
                                GLAMZ SOLUTIONS
                    "Precision Data, Prime Decisions"
================================================================================

1. DESCRIPCIÓN DEL PROYECTO
El sistema funciona como un motor de búsqueda y comparación de artículos de 
consumo masivo. La solución aborda la asimetría de información en el mercado de 
supermercados, entregando al usuario una visualización comparativa de precios, 
ofertas vigentes y disponibilidad de stock en distintas cadenas en tiempo real.

2. PROBLEMÁTICA
Nuestro proyecto se enfoca en resolver la asimetría de información mediante una 
plataforma robusta que permita la trazabilidad de costos. El objetivo principal 
es garantizar la integridad de los datos de usuario y optimizar la eficiencia 
en la toma de decisiones de compra, eliminando la incertidumbre sobre la 
disponibilidad de productos en góndola.

3. DISPOSICIÓN DEL EQUIPO DE TRABAJO
   • Scrum Master:    Enano
   • Product Owner:   René
   • Developers:      Negra
                      Mole
                      Maski

4. CARACTERÍSTICAS DE ENFOQUE / FUNCIONALES
   • Módulo de Autenticación: Sistema centralizado con manejo de sesiones y 
     credenciales cifradas (JWT).
   • Comparativa Multitienda: Procesamiento en paralelo de precios y ofertas 
     de diversas fuentes.
   • Sugerencias Dinámicas: Motor de recomendaciones para minimizar la carga 
     cognitiva del usuario.
   • Monitoreo de Stock Real: Verificación de disponibilidad sincronizada con 
     la realidad de las tiendas.
   • Optimización de Latencia: Consultas de alto rendimiento para despliegue 
     inmediato de resultados.

5. FLUJO DEL USUARIO
   1. Autenticación: Login seguro para personalización y acceso a perfiles.
   2. Dashboard: Panel de ofertas destacadas mediante algoritmos de relevancia.
   3. Búsqueda y Filtro: Selección de artículos y procesamiento de comparación.
   4. Resultados: Visualización de precios, desglose de ofertas y stock.

6. ARQUITECTURA TÉCNICA
   [ CAPA DE CLIENTE (Frontend) ]
          |
          | HTTP/REST (JSON)
          v
   [ CAPA DE ACCESO Y SEGURIDAD (API Gateway) ]
          |-- Auth Service (JWT / Login)
          |-- Rate Limiter (Evita saturación)
          v
   [ CAPA DE LÓGICA DE NEGOCIO (Backend) ]
          |-- Motor de Búsqueda y Sugerencias
          |-- Comparador de Precios (Lógica de ordenamiento)
          |-- Validador de Stock
          v
   [ CAPA DE INTEGRACIÓN (Adaptadores) ]
          |-- Conectores: Lider, Jumbo, Santa Isabel
          v
   [ CAPA DE DATOS ]
          |-- DB Usuarios (PostgreSQL/MySQL)
          |-- Redis (Cache de precios temporal)

7. ATRIBUTOS DE CALIDAD
   • Seguridad (Prioridad Alta): Cifrado y manejo centralizado de sesiones.
   • Usabilidad: Interfaz diseñada para la eficiencia en la búsqueda.
   • Disponibilidad: Core enfocado en la precisión de datos en tiempo real.
   • Rendimiento: Optimización de latencia en consultas distribuidas.

8. PROTOTIPO (FIGMA)
   URL: https://rack-studio-58141370.figma.site/login

================================================================================
 Desarrollado por GLAMZ Solutions para el curso de Bases de Datos I
================================================================================
