# Proyecto-integrado-1

### Descripción del Proyecto
Este proyecto tiene como objetivo analizar datos históricos sobre videojuegos para identificar patrones de éxito, permitiendo a la tienda en línea Ice predecir qué juegos serán prometedores y planificar campañas publicitarias efectivas. El análisis incluye información sobre plataformas, géneros, ventas globales y clasificaciones de usuarios y críticos. Los resultados apoyarán la toma de decisiones estratégicas basada en datos.

El análisis utiliza datos disponibles hasta diciembre de 2016, permitiendo construir un modelo predictivo para las ventas de 2017.

### Objetivos del Proyecto
Preparar los datos: Limpieza y preprocesamiento del conjunto de datos para garantizar la calidad de la información.

Identificar patrones clave: Analizar ventas por plataformas, géneros y regiones.

Examinar factores de éxito: Investigar cómo las clasificaciones de usuarios y críticos influyen en las ventas.

Generar insights accionables: Proponer plataformas y géneros rentables para focalizar las campañas publicitarias.

Probar hipótesis clave: Comparar calificaciones promedio para plataformas y géneros, utilizando pruebas estadísticas.

### Descripción de los Datos
El conjunto de datos incluye las siguientes columnas:

- Name: Nombre del videojuego.
- Platform: Plataforma (e.g., Xbox, PlayStation).
- Year_of_Release: Año de lanzamiento.
- Genre: Género del videojuego.
- NA_sales, EU_sales, JP_sales, Other_sales: Ventas en millones de dólares en Norteamérica, Europa, Japón y otras regiones.
- Critic_Score: Puntuación de críticos (máx. 100).
- User_Score: Puntuación de usuarios (máx. 10).
- Rating: Clasificación ESRB (e.g., Adolescente, Adulto).

### Metodología
Paso 1: Preparación de los Datos
- Conversión de nombres de columnas a minúsculas.
- Conversión de tipos de datos y manejo de valores ausentes:
    - Tratamiento de valores "TBD" (por determinar).
    - Creación de una columna adicional para las ventas totales.
- Descripción de la metodología aplicada para rellenar o dejar en blanco valores ausentes.

Paso 2: Análisis de los Datos
1. Lanzamiento de Juegos:
- Análisis del volumen de lanzamientos por año.
- Evaluación de la relevancia de los datos en distintos períodos.

2. Rendimiento por Plataforma:
- Identificación de plataformas con mayores ventas totales.
- Análisis de ciclos de vida de plataformas populares.

3. Impacto de Reseñas:
- Cálculo de correlación entre las reseñas (usuarios y críticos) y las ventas.
- Comparación de resultados entre plataformas.

4. Distribución por Género:
- Análisis de los géneros más populares y rentables.
- Generalización sobre ventas altas y bajas por género.

Paso 3: Perfil de Usuarios por Región
- Determinación de las 5 plataformas principales en Norteamérica, Europa y Japón.
- Identificación de los 5 géneros más populares en cada región.
- Evaluación del impacto de clasificaciones ESRB en cada mercado.

Paso 4: Pruebas de Hipótesis
  1. Hipótesis 1: Las calificaciones promedio de usuarios para Xbox One y PC son iguales.
  2. Hipótesis 2: Las calificaciones promedio de usuarios para los géneros de Acción y Deportes son diferentes.
     
- Formulación de hipótesis nula y alternativa.
- Selección del criterio de prueba y justificación.

### Conclusión

Comparación de calificaciones entre Xbox One y PC
Resultado: El valor p obtenido fue 0.00058334, que es menor que el nivel de significancia alfa (0.05).
Interpretación: Rechazamos la hipótesis nula, lo que indica que las calificaciones promedio de los usuarios para las plataformas Xbox One y PC no son iguales.
Implicación: Este hallazgo sugiere que los usuarios perciben y califican de manera diferente los juegos en estas dos plataformas. Esto podría deberse a diferencias en la experiencia de usuario, catálogo de juegos, o incluso características técnicas de cada plataforma.

Comparación de calificaciones entre los géneros Acción y Deportes
Resultado: El valor p obtenido fue 1.19440138e-08, significativamente menor que el nivel de significancia alfa (0.05).
Interpretación: Rechazamos la hipótesis nula, indicando que las calificaciones promedio de los usuarios para los géneros de Acción y Deportes son diferentes.
Implicación: Esto muestra una variación en la percepción y satisfacción de los usuarios entre estos géneros. Es probable que los jugadores tengan expectativas diferentes para cada género, o que existan factores externos que influyan en cómo son evaluados.
