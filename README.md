# Análisis de Embudo y Retención por Cohortes en E-commerce
# Descripción del Proyecto 
Este proyecto analiza el comportamiento de los usuarios en una plataforma de comercio electrónico con el objetivo de evaluar la salud del negocio a lo largo de su ciclo de vida. El estudio se divide en dos frentes principales: la identificación de cuellos de botella en el embudo de conversión para entender dónde se pierde la intención de compra, y el análisis de retención por cohortes para medir la recurrencia y fidelización de los clientes a lo largo del tiempo.
# Objetivos de Negocio
* **Mapear el recorrido del usuario:** Cuantificar la progresión y las tasas de caída (drop-off) desde la visualización de productos hasta la transacción final.

* **Evaluar la retención:** Analizar cómo los diferentes grupos de usuarios (cohortes basados en su fecha de registro o primera compra) regresan a la plataforma en los meses posteriores.

* **Generar recomendaciones:** Traducir los hallazgos cuantitativos en acciones estratégicas para optimizar la experiencia de usuario y reducir la fricción en el proceso de pago.
# Stack Tecnológico y Enfoque Metodológico
* **SQL:** Extracción, limpieza y estructuración de los datos transaccionales, mapeando el flujo secuencial de eventos:
  `first_visit` -> `select_item` / `select_promotion` -> `add_to_cart` -> `begin_checkout` -> `add_shipping_info` -> `add_payment_info` -> `purchase`.
  
* **Google Sheets:** Construcción de matrices de retención por cohortes mensuales y aplicación de mapas de calor (*heatmaps*) para visualizar patrones de recurrencia y decaimiento.
# Principales Insights y Recomendaciones
* **Cuello de botella en el embudo:** Se detectó que la transición entre `select_item` y `add_to_cart` concentra el *drop-off* crítico del rendimiento (cayendo del 76.90% al 11.01%), siendo el punto exacto de mayor abandono.
  
* **Estrategia de optimización:** Se prioriza intervenir este tramo mediante el diseño de una **prueba A/B** orientada a reducir la fricción en los pasos previos al pago con el objetivo de lograr un incremento del 15% en la conversión.
  
* **Acciones de retención:** Se complementa la estrategia con acciones correctivas y campañas de *re-engagement* focalizadas en los segmentos con mayor deserción identificados en la matriz de cohortes.
  
