Trucardo version 1.0

Requisitos de instalacion: 
		-Tener Java instalado en tu computadora (Java Runtime Environment)

Instrucciones de ejecucion: 
		- Click derecho sobre el archivo Trucardo.jar
		- Click en Open

Bugs conocidos:
	-En algunas ocasiones es posible que no se pueda cantar Vale Cuatro cuando se tiene el quiero y se debería poder.
	-En algunas manos, la mano se reinicia 2 veces, por lo que se alcanza a ver como cambian las cartas en la mano del jugador.
	-Si se tiene la ventana abierta de detalles, al finalizar la ronda cuando se actualizan los puntos, el fondo de la ventana puede crashear y se debe reiniciar la ventana de detalles.
	-Cuando se canta envido y la AI acepta, en el log primero se imprimen los puntos de los jugadores y luego la respuesta “Quiero” de la AI. Esto debería ser en el orden opuesto.
	-En primera ronda es posible cantar truco y una vez que este es aceptado cantar envido. Una vez que se canta truco no se debería poder cantar envido.

Bugs arreglados:
	-En la segunda mano, cuando la máquina quería jugar una carta se lanzaba una excepción de IndexOutofBounds, la cual crasheaba el programa. Esto fue solucionado y ahora es posible jugar una partida sin problemas.
	-En algunos casos determinados, cuando un jugador cantaba “QUIERO” no se cambiaba de turno adecuadamente, por lo que no se podía avanzar más en la partida y era necesario reiniciarla.
	-En la ventana de detalles, se podía llegar a mostrar que el jugador ganó puntos de truco en una determinada ronda, cuando en realidad no había ganado puntos de truco. Esto ya fue solucionado.
	-Cuando la AI cantaba truco en primer ronda y se le respondía cantando envido, se jugaba el envido y luego seguía el curso de la partida sin haber repuesto el Truco.
	-El log de la mesa en donde se imprimen las acciones había que bajar manualmente la barra. Se corrigió y ahora el log baja automáticamente.

El resto del programa funciona correctamente (creemos).
