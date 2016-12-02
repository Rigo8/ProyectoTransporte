#_Proyecto Transporte_

###En caso de elegir Autobus :bus:

###Las funciones utilizadas son:

* __transporte(Variable):-__

     * Donde recibe un parametro que en caso de ser igual a "autobus", se mostrara un mensaje diciendo que la opcion que ha elegido Posteriormente le preguntara si tiene credencial de estudiante por lo que se debera escribir "si" o "no" como respuesta.
     
* __credencial(Variable):-__ :ticket:

     * Donde recibe un parametro que en caso de ser igual a "si" le dira que debe asegurarse de tener el saldo suficiente por lo que debera responder "si" o "no".  
     * En caso de responder "no" se le preguntara si tiene el dinero suficiente por que debera responder "si"o "no".
     
* __saldo(Variable):-__ :money_with_wings:

    * Donde recibe un parametro que en caso de ser igual a "si" le dira que tome la ruta que lo deje mas cerca de su destino.
    * En caso de responder "no" se le pedira que recargue saldo en en una de las tiendas y posteriormente le estara preguntando si ya recargó hasta que responda que "si".
    
* __dinero(Variable):-__ :moneybag:

    * Donde recibe un parametro que en caso de ser igual a "si" le dira que tome la ruta que lo deje mas cerca de su destino.
    * En caso de responder "no" se le pedira que consiga el dinero suficiente para el autobus y posteriormente le estara preguntando si ya cuenta con el dinero hasta que responda que "si".
    
    :white_circle: :red_circle: Rigo


%Aqui esta las acciones en caso de elegir Autobus
transporte(Transporte):- Transporte='autobus',!,nl,write('Has elegido ir en Autobus! '),nl,write('Tienes credecial de estudiante? '),read(Credencial),credencial(Credencial).
credencial(Credencial):-Credencial='si',!,write('Bien!,asegurate de tener el saldo suficiente, lo tienes? '),read(Saldo),saldo(Saldo).
credencial(Credencial):-Credencial='no',!,write('Entonces, asegurate de tener el dinero suficiente!. Lo tienes? '),read(Dinero),dineroBus(Dinero).

saldo(Saldo):-Saldo='si',!,write('Perfecto!,toma la ruta que te lleve o te deje cerca de tu destino ').
saldo(Saldo):-Saldo='no',!,write('Ve y recarga saldo en una de las Tiendas, ya lo tienes? '),read(SaldoCredencial),saldo(SaldoCredencial).

dineroBus(Dinero):-Dinero='si',write('Perfecto!,toma la ruta que te lleve o te deje cerca de tu destino ').
dineroBus(Dinero):-Dinero='no',write('Consigue el dinero suficiente para el Autobus, lo tienes? '),read(DineroSuficiente),dineroBus(DineroSuficiente).
