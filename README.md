#_ProyectoTransporte_

###Las funciones utilizadas son:
+_viajeEscuela:-_
: Donde no recibira ningun elemento y elegira el transporte en que viajara a la escuela

***
![imagen 1][1]
[1](C://Users/Administrador/Pictures/Proyecto Prolog/transporte.PNG)
viajeEscuela:-write('Elige una forma de transporte'),nl,
	write('auto,uber,autobus'),nl,
	read(Transporte),
	transporte(Transporte).
