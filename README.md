Automatización

Analizar de vídeos publicitarios revisamos las tendencias de vídeos en YouTube para determinar qué contenido merece atención para la mercadotecnia.

Cada video tiene una categoría específica (entretenimiento, música, noticias y política, etc.), una región y una fecha en que se hace tendencia.

Un video puede estar en la sección de tendencias durante varios días seguidos.

Cada semana, consultan esto:

¿Qué categorías estaban en las tendencias de la semana pasada?
¿Cómo se distribuyeron en diversas regiones?
¿Qué categorías fueron particularmente populares en los Estados Unidos?

Hablamos con los administradores de la base de datos y los ingenieros para saber de dónde y cómo se recolectan los datos necesarios, cómo se pueden transformar y dónde almacenar las tablas de agregación. Por último, crearemos el pipeline y el dashboard.

Requisitos técnicos:

Objetivo de negocios: analizar el historial de tendencias de videos en YouTube
Con qué frecuencia se usará el dashboard: al menos una vez al día
Usuario objetivo del dashboard: gerentes de planificación de videos publicitarios
Contenido de los datos del dashboard:
Tendencias pasadas de videos, ordenadas por día y categoría
Tendencias de videos, ordenadas por país
Una tabla de correspondencia entre categorías y países
Parámetros para agrupar los datos:
Fecha y hora de tendencia
Categoría de video
País
Los datos:
Historial de tendencias — valores absolutos ordenados por día (dos gráficos: números absolutos y proporción de porcentaje)
Eventos, ordenados por país — valores relativos (% de eventos)
La correspondencia entre las categorías y los países — valores absolutos (una tabla)
Importancia: todaos los gráficos son igualmente importantes
Fuentes de datos para el dashboard: los ingenieros prometieron crear una tabla de agregación llamada trending_by_time. Esta es la estructura:
record_id: la clave primaria
region: país/región geográfica
trending_date fecha y hora
category_title categoría del video
videos_count número de videos en la sección de tendencias
La tabla está en la base de datos youtube, que se creó especialmente para tus necesidades.
Intervalo de actualización de los datos: una vez cada 24 horas, a la media noche UTC
Gráficos, controles de dashboard y su orden.

