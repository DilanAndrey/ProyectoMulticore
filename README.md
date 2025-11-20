# Pagina de precios de juegos usando web scrapping y multiprocesamiento
<p align="center"> tercer proyecto de arquitectura de computadores </p>.
<p align="center"> desarrollado por: Maikel antonio aguilera camacho, Maria fernanda arce estrada y Dilan andrey sibaja ugalde</p>.

# Vista previa de la pagina
## Pagina al abrirse 
![screenshot de la pagina al abrirse](https://github.com/DilanAndrey/ProyectoMulticore/blob/main/Imagenes/Screenshot%202025-11-19%20183811.png) 
## ejemplo del contenido de cada celda 
![screenshot de ejemplo de tres celdas de juegos](https://github.com/DilanAndrey/ProyectoMulticore/blob/main/Imagenes/Screenshot%202025-11-19%20183843.png) 
## ejemplo del funcionamiento de la barra de busqueda
![screenshot de ejemplo de un juego buscado en la barra de busqueda](https://github.com/DilanAndrey/ProyectoMulticore/blob/main/Imagenes/Screenshot%202025-11-19%20183930.png) 
## Link de la pagina
[CLick aqui para acceder a nuestra pagina](https://dilanandrey.github.io/ProyectoMulticore/)
# acerca del proyecto
el proyecto consiste de un programa desarrollado en python, que le hace web scrapping a distintas paginas para obtener datos de 200 juegos que obtiene de un archivo de texto llamado "lista de juegos.txt", para con esos datos generar una pagina web que sirve como resumen de los precios, calificacion y duracion de cada juego en dicho archivo de texto.
El webdriver utilizado fue selenium, aunque la mayor parte del webscrapping se logra por medio de APIs.
El codigo funciona con multiprocesamiento, pues dos procesos recorren cada mitad del archivo de forma simultanea, y cada uno llama a 3 funciones diferentes que funcionan en paralelo, y 2 que funcionan de manera secuencial, que se encargan de obtener los datos del juego dado para las diferentes paginas que se listan a continuacion.
## paginas a las que hace scrapping
- [steam](https://store.steampowered.com/) paralelo
- [playstation store](https://store.playstation.com/en-us/) paralelo
- nintendo, por medio de este link: https://searching.nintendo-europe.com/es/select. paralelo
- [metacritic](https://www.metacritic.com/) secuencial
- [how long to beat](https://howlongtobeat.com/) secuencial
