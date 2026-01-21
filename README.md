# Analisis-de-datos-de-una-Tienda-de-Videojuegos-Online-
Este análisis exhaustivo del mercado de videojuegos nos permitió comprender cómo las ventas y calificaciones de usuarios varían en función de diferentes factores como plataforma, género, región y clasificaciones ESRB. 
# Introducción
El análisis de datos es una herramienta clave para extraer información valiosa y apoyar la toma de decisiones estratégicas. En este proyecto se analiza un conjunto de datos históricos de ventas de videojuegos de la tienda online Ice, con el objetivo de identificar patrones de comportamiento del mercado, tendencias por plataforma, género y región, así como el impacto de las reseñas de usuarios y críticos.
El proyecto sigue un enfoque estructurado que incluye exploración de datos, procesamiento, pruebas de hipótesis y conclusiones basadas en evidencia estadística.

# Descripción General del Proyecto
La tienda online Ice vende videojuegos a nivel mundial. El dataset contiene información sobre:
Ventas históricas por región
Plataformas y géneros de videojuegos
Reseñas de usuarios y críticos
Clasificación por edades según ESRB

La clasificación ESRB (Entertainment Software Rating Board) evalúa el contenido de los videojuegos y asigna categorías de edad como Everyone (E), Teen (T) o Mature (M).
Nota: Los datos correspondientes al año 2016 pueden estar incompletos.

# Descripción del Dataset
Columnas del Dataset:
Name: Nombre del videojuego
Platform: Plataforma
Year_of_Release: Año de lanzamiento
Genre: Género
NA_sales: Ventas en Norteamérica (millones USD)
EU_sales: Ventas en Europa (millones USD)
JP_sales: Ventas en Japón (millones USD)
Other_sales: Ventas en otras regiones (millones USD)
Critic_Score: Puntuación de críticos (0–100)
User_Score: Puntuación de usuarios (0–10)
Rating: Clasificación ESRB

Durante la exploración inicial se identificaron valores faltantes, especialmente en Critic_Score, User_Score, Rating y Year_of_Release, los cuales fueron considerados durante el procesamiento de datos.

# Objetivos del Proyecto
Este análisis busca responder las siguientes preguntas:
¿Cómo ha evolucionado el lanzamiento de videojuegos a lo largo del tiempo?
¿Qué plataformas han sido líderes en ventas y cuáles han perdido relevancia?
¿Qué período de datos es más adecuado para construir un modelo predictivo para 2017?
¿Qué plataformas y géneros son potencialmente más rentables?
¿Existen diferencias significativas en las calificaciones de usuarios entre plataformas y géneros?
¿Qué impacto tienen las reseñas de críticos y usuarios en las ventas?

# Metodología y Etapas del Análisis
El proyecto se desarrolló siguiendo estas etapas:
1 Exploración y descripción de los datos
2 Procesamiento y limpieza de datos
3 Análisis exploratorio (EDA)
4 Análisis de ventas por plataforma, género y región
5 Pruebas de hipótesis
6 Conclusiones y recomendaciones

# Pruebas de Hipótesis
Comparación de Géneros: Acción vs. Deportes
Hipótesis Nula (H₀):
Las calificaciones promedio de los juegos de Acción y Deportes son iguales.
Hipótesis Alternativa (H₁):
Las calificaciones promedio de los juegos de Acción y Deportes son diferentes.
Tipo de prueba: Bilateral (two-tailed)
Nivel de significancia: α = 0.05
Resultados
Media Acción: 7.05
Media Deportes: 6.96
Mediana en ambos géneros: 7.4
Aunque las medias y medianas son muy similares, la prueba estadística indicó diferencias significativas en la distribución de las calificaciones, lo que sugiere que la forma en que los usuarios valoran estos géneros es distinta.

Comparación de Plataformas: Xbox One vs. PC
Se rechazó la hipótesis nula.
Existen diferencias significativas en las calificaciones de usuarios entre ambas plataformas, posiblemente relacionadas con expectativas distintas según el tipo de jugador.

# Resultados del Análisis
Tendencias del Mercado
PS4 y Xbox One dominaron las ventas en los años más recientes.
Consolas históricas como PS2 y Wii mostraron un descenso notable.
Las plataformas suelen alcanzar su pico de ventas entre los 5 y 6 años de vida.
Los géneros más populares fueron Acción, Deportes y Disparos.
Los géneros Rol y Aventura mostraron crecimiento constante.

# Análisis Regional
América del Norte (NA):
Dominio de PS4, Xbox One y Wii
Alta preferencia por juegos de Acción y Deportes
Mayor volumen de ventas en juegos con clasificación E.
Europa (EU):
Mayor diversidad de plataformas y géneros
Fuerte presencia de juegos de Rol y Carreras
Japón (JP):
Dominio de plataformas de Nintendo
Preferencia por géneros de Rol y Aventura
Menor impacto de clasificaciones T y M

# Impacto de las Reseñas
Correlación ventas–críticos: 0.41 (moderada)
Correlación ventas–usuarios: -0.03 (casi nula)
Esto indica que las reseñas profesionales influyen más en las decisiones de compra que las opiniones de los usuarios.

# Comparación de Ventas Multiplataforma
Juegos lanzados en múltiples plataformas (por ejemplo Alien: Isolation y Assassin’s Creed IV: Black Flag) mostraron mejores ventas en consolas, especialmente PS4, en comparación con PC.

# Conclusiones Generales
El análisis confirma que el desempeño comercial de los videojuegos está fuertemente influenciado por:
La plataforma
El género
La región
La crítica profesional
Aunque las calificaciones promedio entre géneros pueden ser similares, las diferencias en distribución y dispersión reflejan experiencias de usuario distintas. Comprender estas dinámicas permite a desarrolladores y distribuidores optimizar estrategias de lanzamiento, marketing y selección de plataformas, aumentando las probabilidades de éxito comercial.

# Herramientas Utilizadas
Python
Pandas
Análisis Exploratorio de Datos (EDA)
Estadística descriptiva
Pruebas de hipótesis
