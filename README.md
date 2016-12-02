#_ProyectoTransporte_

###Las funciones utilizadas son:
+_viajeEscuela:-_
: Donde no recibira ningun elemento y elegira el transporte en que viajara a la escuela

***
![1](pictures/proyectoProlog/transporte.PNG)
viajeEscuela:-write('Elige una forma de transporte'),nl,
	write('auto,uber,autobus'),nl,
	read(Transporte),
	transporte(Transporte).
