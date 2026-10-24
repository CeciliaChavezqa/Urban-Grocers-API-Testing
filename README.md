# Urban-Grocers-API-Testing 
🔗 Proyecto de QA: API Testing - Urban Grocers
## 📝 Descripción
Urban Grocers es un ejemplo de plataforma interactiva de comercio electrónico enfocada en la entrega de productos por catálogo y kits preparados. El objetivo principal de este proyecto fue realizar pruebas de backend (API Testing) sobre los microservicios críticos de la plataforma para asegurar la integridad de las operaciones de negocio, la correcta validación de esquemas de datos y el funcionamiento óptimo de la lógica de entregas y kits.

## 🛠️ Tecnologías y Herramientas
Postman: Utilizado para la construcción, ejecución, pruebas parametrizadas y validación de respuestas de los endpoints de la API.

Lenguaje de Scripting: JavaScript (para tests automáticos dentro de Postman).

Documentación de la API: Documentación oficial de Urban Grocers.

Jira: Gestión de incidencias, creación de reportes de errores (Bug Reports) detallados con severidad, pasos para reproducir y resultados esperados/obtenidos.

Excel: Diseño estructurado de Casos de Prueba (pruebas de límites, clases de equivalencia y flujos negativos/positivos).

Entorno: Servidores remotos de TripleTen.

Protocolo: REST (JSON).

## 🔍 ¿Qué se probó? (Alcance)
El proyecto se centró en la validación exhaustiva de dos módulos principales del backend:

🛒1. Gestión de Kits (/api/v1/kits): 

Creación, consulta, modificación (renombrado y actualización de productos) y eliminación de kits.

Validación de restricciones en los nombres de los kits (solo letras latinas, espacios y guiones, longitud de 2 a 15 caracteres) y límite de artículos (máximo 30).

🛒2. Servicios de Entrega y Logística (/api/v1/couriers, /api/v1/orders, etc.):

Verificación de disponibilidad de servicios de entrega automáticos y manuales (Speedy, Fast Delivery, Food Service, Order and Go, etc.).

Validación del cálculo de costos internos (host delivery cost) y para el cliente (client delivery cost) en función del peso total, cantidad de artículos y horarios de operación.

Reglas de negocio para envíos automáticos (costo fijo de $5 USD por exceso de peso, cantidad o montos menores a $7 USD).

## 📋 Tipos de Casos Cubiertos
Se diseñó e implementó una suite de pruebas abarcando:

Pruebas Positivas (Happy Path): Verificación de que el sistema responde con códigos 200/201 y la estructura de datos correcta ante solicitudes válidas de kits y consultas de couriers.

Pruebas Negativas: Validación del manejo de errores ante datos fuera de rango (ej. nombres de kits con caracteres especiales o longitudes inválidas, exceso de peso permitido por los couriers, formatos incorrectos).

Pruebas de Límites (Boundary Value Analysis): Evaluación estricta en los umbrales de peso y cantidad de artículos por pedido (ej. límites exactos para cobros de envíos automáticos y tarifas de transportistas específicos).

## 💡 Nuevas competencias adquiridas 
Profundizar en el análisis de requerimientos de backend complejos para traducirlos en matrices de pruebas estructuradas.

Manejo de distintos formatos de intercambio de datos requeridos por proveedores logísticos externos dentro de una API (JSON, XML).

Documentación de incidencias de forma técnica y profesional en herramientas de seguimiento como Jira, facilitando la comunicación asertiva con el equipo de desarrollo.

## 📂 Evidencias para Revisar

Casos de Prueba: **"Proyecto para el 4.º Sprint_ Ejercicio.xlsx"**

<img width="1865" height="672" alt="image" src="https://github.com/user-attachments/assets/7fb38f16-fc54-4724-999c-5fa28129a187" />


## 👤 Autor

**Cecilia Mena Chavez | Ingeniera en Tecnología Automotriz | QA Engineer**
"Transformando la precisión técnica en software confiable."
