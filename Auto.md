#_ProyectoTransporte_
###En caso de elegir auto

###Las funciones utilizadas son:
* _transporte(Variable):-_
        : Donde recibe un parametro que en caso de ser igual a "auto", se mostrara un mensaje diciendo que la opcion que ha elegido. Posteriormente le mostrara un mensaje pidiendole que busque sus llaves y se le preguntara si cuenta con ellas por lo que se debera escribir "si" o "no" como respuesta.

* _encontrarLlaves(Variable):-_
        1. Donde recibe un parametro que en caso de ser igual a "si" le dara acceso al siguiente paso y le pedira que busque su licencia.
Posteriormente le preguntara si tiene su licencia, donde debera responder si o no.
        2. En caso de responder "no" se estara ejecutando la funcion hasta que su respuesta sea "si".
        
        
transporte(Transporte):- Transporte='auto',!,nl,write('Has elegido ir en Auto!'),nl,write('Busca las llaves!, ya las tienes '),read(Llaves),encontrarLlaves(Llaves).
encontrarLlaves(Llaves):- Llaves='si',!,write('Bien!, Continua el siguiente paso '),nl,write('Tienes tu licencia '),read(Licencia),licencia(Licencia).
encontrarLlaves(Llaves):- Llaves='no',!,write('Sigue buscando, Ya las encontraste? '), read(Respuesta),encontrarLlaves(Respuesta).
licencia(Licencia):- Licencia='si',!,write('Excelente!, Ahora al siguiente paso '),nl,write('Recuerda usar el Cinturon de Seguridad, Lo tienes? '),read(Paso),dentro(Paso).
licencia(Licencia):- Licencia='no',!,write('Muy mal!, Sigue buscando. Ya la tienes? '),read(Respuesta),licencia(Respuesta).

dentro(Respuesta):- Respuesta='si',!,write('Ahora enciende el auto y ve con precaucion ').
dentro(Respuesta):- Respuesta='no',!,write('Usalo, para prevenir algun daño en caso de accidente, Ya lo tienes? '),read(Cinturon),dentro(Cinturon).
