#_ProyectoTransporte_

###Las funciones utilizadas son:
1. viajeEscuela
	*Donde no recibira ningun elemento y elegira el transporte en que viajara a la escuela


viajeEscuela:-write('Elige una forma de transporte'),nl,
	write('auto,uber,autobus'),nl,
	read(Transporte),
	transporte(Transporte).
