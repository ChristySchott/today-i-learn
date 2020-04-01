# Modo estrito

O ES5 adicionou o "strict mode" para a linguagem, que determina regras mais rígidas para certos comportamentos. Geralmente essas restrições são vistas como algo que faz o código se tornar mais seguro e com padrões melhor definidos. Além disso, aderindo ao modo estrito, em geral, seu código será melhor otimizado pelo Motor. O strict mode é uma grande vitória para o código, e você deveria usá-lo em todos os seus programas.

Você pode optar pelo modo estrito em uma função individualmente, ou em todo um arquivo, dependendo de onde você determinar o pragma do modo estrito:

```
function foo() {
    "use strict";

    // este código usa o modo estrito

    function bar() {
        // este código está em modo estrito
    }
}

// este código não está em modo estrito
```

Compare isso com:

```
"use strict";

function foo() {
    // este código está em modo estrito

    function bar() {
        // este código está em modo estrito
    }
}

// este código está em modo estrito
```

Uma diferença chave (melhoria!) com o strict mode é desabilitar a variável auto-global implícita ao omitir o var:

```
function foo() {
    "use strict";   // liga o strict mode
    a = 1;          // `var` faltando: ReferenceError
}

foo();
```

Se você habilitar o modo estrito em seu código, e você receber erros, ou o código se comporta de maneira bugada, a tentação é evitar o modo estrito. Mas esse instinto é uma má ideia de se deixar acontecer. Se o modo estrito gera problemas no seu programa, é certo que isso é um sinal que existem coisas que você deve consertar.

O modo estrito não irá apenas deixar seu código em um caminho mais seguro, também deixará seu código mais otimizável e também representando o futuro da linguagem. É mais fácil se acostumar com o modo estrito agora do que deixá-lo de lado -- vai ser mais difícil se converter a ele mais tarde!
