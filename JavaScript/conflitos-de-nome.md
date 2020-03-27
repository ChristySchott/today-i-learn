# Conflitos de nome 




Quando dois argumentos ou variáveis nos escopos da closure **(se não sabe o que é uma closure, procure nesse mesmo repositório)** tem o mesmo nome, há um conflito de nome. Mas escopos internos tem maior prioridade, enquanto que o escopo mais externo tem a menor. Na "cadeia do escopo", o primeiro da cadeia é o escopo mais interno, e o último é o escopo mais externo. 

## Exemplo:

    function fora() {
       var x = 10;
       function dentro(x) {
      return x;
       }
       return dentro;
    }
    result = fora()(20); // retorna 20 em vez de 10


O conflito de nome acontece na declaração return x mas como o x de dentro tem preferência e o 20 é declarado dentro dele, é o 20 que retorna. 