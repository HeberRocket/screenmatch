# Este es un código Java con ayuda del framework spring, es una aplicación de consola que interactúa con la API de OMDB (The Open Movie Database) para obtener información sobre series de televisión y episodios.

## Importaciones de clases y paquetes: 

El código importa varias clases y paquetes necesarios para el funcionamiento del programa, 
incluyendo clases para manejar la entrada del usuario, consumir una API web, y convertir datos JSON en objetos Java.

## Método muestraElMenu():

Este método es el punto de entrada del programa. Imprime un mensaje pidiendo al usuario 
que ingrese el nombre de una serie de televisión que desea buscar.

## Obtención de datos de la serie:

El nombre de la serie ingresado por el usuario se utiliza para realizar una consulta a la API de OMDB y obtener 
datos generales sobre la serie, como su título, año de inicio, género, etc.

## Obtención de datos de temporadas:

Después de obtener los datos generales de la serie, el programa busca información sobre cada temporada de la serie 
haciendo múltiples consultas a la API, una para cada temporada. Los datos de cada temporada se almacenan en una lista.

## Procesamiento de episodios:
Una vez que se han obtenido los datos de todas las temporadas, el código deserializa lso datos convirtiendo el json en clases java con ayuda del jackson, combinando todos los episodios en una sola lista de objetos DatosEpisodio.

## Análisis de los episodios:
El código realiza varias operaciones con la lista de episodios, como filtrar los episodios sin evaluación, calcular el promedio 
de las evaluaciones por temporada, y encontrar el episodio mejor y peor evaluado.

## APIKEY
Para obtener tu api_key debes ingresar a la pagina oficial de Omdb: https://www.omdbapi.com/
