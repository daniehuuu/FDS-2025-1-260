# Objetivo del proyecto
El objetivo principal del análisis es identificar las tendencias y preferencias de los usuarios en YouTube en Alemania, atendiendo a aspectos como la categoría del contenido, la actividad de los canales, el comportamiento por región y la evolución temporal. Se busca resolver preguntas relacionadas con qué tipos de videos generan más interacción, cuáles son más apreciados o rechazados, qué canales se destacan en popularidad y si es posible anticipar métricas como vistas, “Me gusta” y “No me gusta”. El conocimiento a estimar incluye patrones de consumo, indicadores de popularidad y señales predictivas sobre el comportamiento de las audiencias.

# Nombre de los participantes

- Abanto Davila Alvaro Jair Moises (u202313540)
- Cuadrado Jimenez Sebastian Antonio (u202312882)
- Huapaya Vargas Daniel José (u202312230)

# Descripción del conjunto de datos

| Columna                | Tipo de Dato                | Descripción                                                                                   |
|------------------------|----------------------------|-----------------------------------------------------------------------------------------------|
| video_id               | Categórico (Nominal)       | Identificador único alfanumérico del video. No tiene orden ni jerarquía.                      |
| trending_date          | Categórico (Fecha), Ordinal| Fecha en formato DD.MM.YY.                                                                    |
| title                  | Categórico (Nominal)       | Título del vídeo. Texto libre sin categorización predefinida.                                 |
| channel_title          | Categórico (Nominal)       | Nombre del canal. No tiene orden jerárquico.                                                  |
| category_id            | Numérico (Discreto)        | ID de la categoría del video. Usado como etiqueta categórica (nominal).                       |
| publish_time           | Categórico (Fecha, Ordinal)| Marca de tiempo de publicación (ISO).                                                         |
| tags                   | Categórico (Nominal)       | Lista de etiquetas separadas por pipes (|). Cada tag es una categoría nominal.                |
| views                  | Numérico (Discreto)        | Número total de vistas. Solo valores enteros.                                                 |
| likes                  | Numérico (Discreto)        | Cantidad de "Me gusta". Valores enteros no negativos.                                         |
| dislikes               | Numérico (Discreto)        | Cantidad de "No me gusta". Valores enteros no negativos.                                      |
| comment_count          | Numérico (Discreto)        | Número de comentarios. Entero no negativo.                                                    |
| thumbnail_link         | Categórico (Nominal)       | URL de la miniatura. No tiene orden ni significado numérico.                                  |
| comments_disabled      | Categórico (Bool)          | Indica si los comentarios están desactivados (True/False).                                    |
| ratings_disabled       | Categórico (Bool)          | Indica si los ratings (likes/dislikes) están desactivados (True/False).                       |
| video_error_or_removed | Categórico (Bool)          | Indica si el video tiene errores o fue eliminado (True/False).                                |
| description            | Categórico (Nominal)       | Descripción textual del video. No categorizable.                                              |
| state                  | Categórico (Nominal)       | Nombre del Estado/región de Alemania. Sin orden jerárquico.                                   |
| lat                    | Numérico (Continua)        | Latitud geográfica del Estado. Valor decimal con precisión.                                   |
| lon                    | Numérico (Continua)        | Longitud geográfica del Estado. Valor decimal con precisión.                                  |
| geometry               | Categórico (Geo, Nominal)  | Coordenadas en formato POINT. Útil para mapeo geoespacial (GeoPandas).                        |

# Conclusiones

1. La gráfica muestra que las categorías de videos con mayor número de registros en tendencia son principalmente Entertainment y People & Blogs, seguidas por News & Politics, Sports y Comedy. Esto indica que el contenido de entretenimiento y blogs personales domina la popularidad en YouTube Alemania, reflejando el interés de la audiencia por temas ligeros, actualidad y experiencias personales. Las categorías menos representadas, como Trailers, Movies y Shows, tienen una presencia mucho menor en las tendencias, lo que sugiere que estos temas generan menos contenido viral o de alto impacto en la plataforma.

2. La exploración y análisis de los datos de tendencias de YouTube en Alemania revela que ciertas categorías, como "Music", "Comedy" y "Movies", tienden a generar mayor interacción positiva y volumen de likes, mientras que otras presentan menor engagement. Este insight puede guiar a creadores de contenido y marcas a enfocar sus esfuerzos en categorías con mayor potencial de viralidad y preferencia del público, optimizando así sus estrategias de contenido y campañas publicitarias para maximizar el alcance y la interacción en la plataforma.

3. Las categorías de video con mayor ratio de “Me gusta” respecto a “No me gusta” reflejan una alta aceptación y bajo nivel de controversia entre los usuarios. Esto indica que el contenido en dichas categorías genera consenso y satisfacción, siendo ideal para estrategias de marketing que buscan maximizar la aprobación del público y minimizar el riesgo reputacional.

4. Las categorías de video con mayor ratio de “Me gusta” respecto a “No me gusta” reflejan una alta aceptación y bajo nivel de controversia entre los usuarios. Esto indica que el contenido en dichas categorías genera consenso y satisfacción, siendo ideal para estrategias de marketing que buscan maximizar la aprobación del público y minimizar el riesgo reputacional.

5. Para el negocio, esto indica que la plataforma ofrece una oportunidad constante para que los creadores logren visibilidad. Se recomienda mantener una estrategia de publicación regular y monitorear los días con menor volumen, ya que podrían representar ventanas de menor competencia y mayor probabilidad de destacar en tendencias. Además, analizar las causas de las caídas puede ayudar a anticipar cambios en el algoritmo o en la dinámica de la plataforma.

6. Los canales que aparecen más frecuentemente en tendencia destacan por su capacidad de generar contenido relevante y mantener una audiencia activa, lo que los convierte en aliados estratégicos para campañas de marketing digital. Por otro lado, los canales con menor frecuencia pueden pertenecer a nichos específicos o tener menor visibilidad, pero representan oportunidades para segmentar audiencias o explorar mercados menos saturados.

7. 
    - Likes: Los cinco estados con más "Me gusta" son Hamburg, Bremen, Hessen, Berlin y Thuringen. Esto indica que en estos estados la audiencia tiende a reaccionar positivamente al contenido, mostrando alto nivel de aprobación.
    - Vistas: Los cinco estados con más visualizaciones son Hamburg, Thuringen, Rheinland Pfalz, Hessen y Schleswig Holstein. Esto refleja que en estos lugares se concentra el mayor consumo de videos en YouTube, probablemente por su tamaño poblacional o actividad digital.
    - Dislikes: Los cinco estados con más "No me gusta" son Thuringen, Schleswig Holstein, Hamburg, Hessen y Bremen. Aquí se observa que algunos estados que lideran en vistas y likes también tienen una audiencia crítica o polarizada.  
  
8. Para el negocio, esto indica que la plataforma ofrece una oportunidad constante para que los creadores logren visibilidad. Se recomienda mantener una estrategia de publicación regular y monitorear los días con menor volumen, ya que podrían representar ventanas de menor competencia y mayor probabilidad de destacar en tendencias. Además, analizar las causas de las caídas puede ayudar a anticipar cambios en el algoritmo o en la dinámica de la plataforma.

9. La predicción del número de vistas es factible y aporta valor para anticipar el alcance potencial de los videos, pero su precisión es limitada por la complejidad y diversidad de los contenidos en YouTube. Para mejorar la exactitud, sería recomendable incorporar más variables y técnicas avanzadas de modelado. Este resultado es útil para orientar estrategias de marketing digital y optimizar la publicación de contenidos en función de las tendencias observadas.

# Lincencia de uso
Este proyecto está licenciado bajo la Licencia MIT. 