# Expressões de Função Invocadas Imediatamente (IIFEs)

> * Trechos retirados do livro You Dont Know JS


Existe uma outra forma de executar uma expressão de função, que é tipicamente chamada de Expressões de Função Invocadas Imediatamente (immediately invoked function expression, ou IIFE):

```
(function IIFE(){
    console.log( "Hello!" );
})();
// "Hello!"
```

O ( .. ) externo que rodeia a expressão de função (function IIFE(){ .. }) é apenas uma nuance que a gramática do JS precisa para prevenir que seja tratada como uma declaração de uma função qualquer.

O final () no fim da expressão -- a linha })(); -- é o que atualmente executa a expressão da função referenciada logo em seguida a ela.

Isso pode parecer estranho, mas não é tão desconhecido em um primeiro olhar. Considere as similaridades entre foo e IIFE abaixo:

```
function foo() { .. }

// referência de expressão `foo`,
// depois `()` executa ele
foo();

// expressão da função `IIFE`,
// depois `()` executa ele
(function IIFE(){ .. })();
```

Como você pode ver, listar (function IIFE(){ .. }) antes de sua execução () é essencialmente a mesma coisa do que executar foo antes de sua execução (); em ambos os casos, a referência da função é executada com o () logo em seguida.

Porque IIFE é apenas uma função, e funções criam variáveis scope, usar uma IIFE dessa forma é muitas vezes usado para declarar variáveis que não afetarão o código fora de IIFE:

```
var a = 42;

(function IIFE(){
    var a = 10;
    console.log( a );   // 10
})();

console.log( a );       // 42
```

IIFEs também podem retornar valores:

```
var x = (function IIFE(){
    return 42;
})();

x;  // 42
```

O valor 42 é retornado da função nomeada IIFE, e depois designada à variável x.
