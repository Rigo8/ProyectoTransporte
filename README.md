# ProyectoTransporte
Proyecto de Programacion Logica

%Aqui se esta eligiendo la opcion en que ira a la escuela.

viajeEscuela:- write('Elige una forma de transporte'),nl,
	write('auto,uber,autobus'),nl,
	read(Transporte),
	transporte(Transporte).
