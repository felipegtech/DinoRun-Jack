# 🦖 Dino Cloud Climber (Nand to Tetris - Proyecto 9)

Este es un juego desarrollado en el lenguaje Jack para la plataforma de hardware Hack, como parte de la materia de Organización de Computadores.

Es un juego de salto y supervivencia vertical donde controlas a un dinosaurio que debe trepar nubes. A diferencia de un juego lateral tipo "Endless Runner", en esta versión el objetivo no es esquivar obstáculos, sino saltar de nube en nube para seguir subiendo.

El mundo se desplaza constantemente, simulando que el dinosaurio asciende por una ruta de nubes. El jugador debe presionar la barra espaciadora en el momento correcto para que el dinosaurio salte hacia la siguiente nube. Si no salta a tiempo o cae fuera de la pantalla, pierde la partida.

El proyecto demuestra el uso de programación orientada a objetos en Jack, manejo de memoria, gráficos por bloques, simulación básica de físicas, detección de aterrizajes y lectura de periféricos como el teclado.

## 🚀 Cómo jugar

Dado que el juego está escrito en Jack, necesita compilarse a código de Máquina Virtual (.vm) y ejecutarse en el emulador oficial del curso Nand to Tetris.

## Requisitos previos

Descargar las herramientas oficiales del curso Nand to Tetris.  
Tener el JackCompiler y el VMEmulator listos para usar.

## Ejecución

Compila la carpeta completa del proyecto usando el JackCompiler.

Abre el VMEmulator.

Haz clic en el ícono de "Load Program" 📂 y selecciona la carpeta completa de este proyecto.

⚠️ MUY IMPORTANTE: En las opciones del emulador, desactiva las animaciones (No animation) y pon la velocidad al máximo (Fast).

Dale al botón de ejecución rápida (⏩).

## 🎮 Controles

Barra Espaciadora: Saltar hacia la siguiente nube.  
Tecla 'Q': Salir del juego.

## 🏗️ Arquitectura del Código

El juego está dividido en 4 clases principales para separar las responsabilidades:

Main.jack: Punto de entrada del programa. Inicializa el juego y limpia la memoria al terminar.

DinoGame.jack: Es el motor principal. Maneja el bucle infinito (Game Loop), la puntuación, el movimiento del mundo, el avance de las nubes y la detección de aterrizajes.

Dino.jack: Controla al jugador (el dinosaurio). Contiene las físicas simuladas de gravedad, la fuerza del salto, el cálculo automático hacia la siguiente nube y las coordenadas de dibujo de la figura.

Obstacle.jack: Controla las nubes/plataformas. Maneja su dibujo, movimiento en pantalla y reaparición cuando salen del área visible.

## 🛠️ Tecnologías

Lenguaje: Jack (Alto nivel, orientado a objetos).  
Plataforma: Hack Virtual Machine.
  ![Demo del Juego](assets/GameDemo.png)
