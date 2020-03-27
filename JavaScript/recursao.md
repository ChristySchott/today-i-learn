# Recursão




Uma função que chama a si mesma é chamada de **função recursiva**. Há 3 maneiras de uma função chamar a si mesma:

- usando o nome dela
- usando o comando  '*arguments.callee*'
- uma variavel que se refere a ela no mesmo escopo**

> ** var pessoa = function homem() {
 
Nesse caso acima, posso retornar a  função **homem** chamando a variável **pessoa**.



  

## Exemplo:
##### O *while:*

        var x = 0;
    while (x < 10) { // "x < 10" a condição do laço
       // faça coisas
       x++;
    }


##### Vai ser convertido em função recursiva:*

       function loop(x) {
       if (x >= 10) // "x >= 10" a condição de parada (equivalente a "!(x < 10)")
       return;
       // faça coisas
       loop(x + 1); // chamada recursiva
       }
       loop(0);