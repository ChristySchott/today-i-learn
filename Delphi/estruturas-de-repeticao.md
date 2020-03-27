# Estruturas de Repetição	

Começando os estudos sobre Delphi, tive facilidade com as estruturas de repetição, pois é semelhante ás estruturas de outras linguagens.

#### For:
executa repetitivamente um comando enquanto é atribuído um valor incremental a uma variável de controle, que chamamos de contador do for. A repetição, ou o loop só é interrompido quando o contador atinge o seu limite, que é definido também pela instrução for.

Sintaxe:

    1. for variável := <início> to/downto <fim> do
    2.<instrução a ser repetida>;

ou (com mais de uma instrução):

    1. for variável := <início> to/downto <fim> do
    2. begin
    3.<instrução a ser repetida 1>;
    4.<instrução a ser repetida 2>;
    5.<instrução a ser repetida 3>;
    6.<…>
    7. end;

Onde:
variável = contador do for, qualquer valor inteiro.

inicio = valor a partir do qual o loop deve iniciar, qualquer valor inteiro.

fim = valor limite para o término do loop, qualquer valor inteiro.

###### Somando até 10:

    1. procedure Somar;
    2. var
    3. Contador, Soma: Integer;
    4. begin
    5. Soma := 0;
    6. for Contador := 1 to 10 do
    7. Soma := Soma + 1;
    8. end;

To declarando duas variáveis, a Soma e o Contador. Esta última estou usando como controlador para o laço. O loop será de 0 a 10.


----------

#### While..do:
 tem o seu funcionamento controlado por condição. Desta forma, poderá executar um determinado conjunto de instruções enquanto a condição verificada permanecer verdadeira.

No momento em que a condição se torna falsa, o processamento da rotina é desviado para fora do loop. Se a condição for falsa logo no início do loop, as instruções contidas no while…do serão ignoradas.

Sintaxe:

       1. while <condição> do
       2.<instrução a ser repetida para condição verdadeira>;

ou (com mais de uma instrução):

       1. while <condição> do
       2. begin
       3.<instrução a ser repetida para condição verdadeira 1>;
       4.<instrução a ser repetida para condição verdadeira 2>;
       5.<instrução a ser repetida para condição verdadeira 3>;
       6.<…>
       7. end;

###### Somando até 10:
	    
	   1. procedure Somar;
	   2. var
	   3. Soma: Integer;
	   4. begin
	   5. Soma := 0;
	   6. while Soma <= 10 do
       7. Soma := Soma + 1;
       8. end;

----------

#### Repeat..until:
  é parecida com a estrutura while…do, mas a principal diferença entre elas, é que no repeat…until, o teste lógico é efetuado no final do loop.

Essa estrutura irá processar um conjunto de instruções até que a condição se torne verdadeira. 

Sintaxe:

    1. repeat
    2.<instrução a ser repetida até que a condição seja verdadeira 1>;
    3.<instrução a ser repetida até que a condição seja verdadeira 2>;
    4.<instrução a ser repetida até que a condição seja verdadeira 3>;
    5.<…>
    6. until
    7.<condição>;



###### Somando até 10:
	    
	   1. procedure Somar;
	   2. var
	   3. Soma: Integer;
	   4. begin
	   5. Soma := 0;
	   6.  repeat 
	   7.    Soma := Soma + 1;
	   7.  until 
	   8.    Soma <= 10;
       8. end;
