# Variáveis no Delphi

##### BOOLEAN:
  Tipo lógico que pode assumir somente os valores TRUE ou FALSE e ocupa 1 byte de memória.

##### BYTE: 
Tipo numérico inteiro, pode assumir valores numa faixa de  0 a 255, ocupa 1 byte.

##### CHAR: 
Tipo alfa-numérico, pode armazenar um caractere ASCII,  ocupa 1 byte.

##### COMP: 
Tipo numérico real, pode assumir valores na faixa de -9,2×10-18  a 9,2×10+18. Ocupa 8 bytes, pode ter entre 19 e 20 algarismos significativos.

##### EXTENDED: 
Tipo numérico real, pode assumir valores na faixa de -3,4×10-4932  a +1,1×10+4932. Ocupa 10 bytes de memória e tem entre 19 e 20 algarismos significativos.

##### INTEGER: 
Tipo numérico inteiro, pode assumir valores numa faixa de  -32768 a +32767, ocupa 2 byte de memória.

##### LONGINT:
 Tipo numérico inteiro, pode assumir valores numa faixa de  -2147483648 a +2147483647, ocupa 4 bytes de memória.

##### REAL:
 Tipo numérico real, pode assumir valores na faixa de -2,9×10-39  a +1,7×10+38. Ocupa 6 bytes de memória e tem entre 11 e 12 algarismos significativos.

##### SHORTINT: 
Tipo numérico inteiro, pode assumir valores numa faixa de  -128 a +127, ocupa 1byte de memória.

##### SINGLE: 
Tipo numérico real, pode assumir valores numa faixa de  -1,5×10-45  a +3,4×10+38. Ocupa 4 bytes de memória, e tem de 7 a 8 algarismos significativos.

##### WORD: 
Tipo numérico inteiro, pode assumir valores numa faixa de  0 a 65535, ocupa 2bytes de memória.

##### STRING: 
Tipo alfanumérico, possuindo como conteúdo uma cadeia de caracteres. O número de bytes ocupados na memória varia de 2 a 256. Dependendo da quantidade máxima de caracteres definidos para a string. O primeiro byte contém a quantidade real de caracteres da cadeia.


----------

Ao iniciar um projeto no Delphi haverá duas possibilidades para declarar um variável, *private* ou *public*. Se ela for privada não poderei usar em outros arquivos.

#### Definindo uma var:

    private
    
    var quantidade: Double;

#### Atribuindo um valor a essa var:

    quantidade := 1090;

Quando eu for apresentar essa variável usando o ShowMessage(); tenho que ter cuidado para convertê-la para o tipo String, pois é o unico que esse método aceita.

Então ficaria assim:

    ShowMessage(FloatToStr(quantidade));