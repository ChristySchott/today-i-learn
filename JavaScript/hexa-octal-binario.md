# toString()

Com o comando toString() podemos definir se iremos apresentar o valor de um numero em decimal, hexadecimal, octal ou binário, por exemplo.

Criarei a varivel *numero* e atribuirei um valor de 32 a ela, em seguida iremos apresentá-lo de um modo diferente com a função toString()

> var numero = 32;

> window.alert(numero.toString(10))      
//aqui é decimal então o valor apresentando será **32**


> window.alert(numero.toString(16))       
//aqui é hexadecimal então o valor apresentando será **20**


> window.alert(numero.toString(8))       
//aqui é octal então o valor apresentando será **40**


> window.alert(numero.toString(2))        
//aqui é binário então o valor apresentando será **100000**

