# Closures


O JavaScript permite o aninhamento de funções e garante  à função interna o acesso completo a todas as variáveis e funções definidas dentro da função externa (e todas as outras variáveis e funções que a função externa tem acesso). Porém, a função externa não tem acesso às variáveis e funções definidas dentro da função interna. Isto garante uma maior segurança para as variáveis da função interna. Além disso, uma vez  que a função interna tem acesso ao escopo da função externa, as variáveis e funções definidas na função externa vão durar na memória mais do que a própria função externa, isto se a função interna permanecer na memória mais tempo do que a função externa. Uma **closure** é criada quando a função interna é de alguma forma disponibilizada para qualquer escopo fora da função externa.

## Exemplo de closure:

    var pessoa = function(nome) {  // Função externa
      var getNome = function() {
      return nome; // Função interna tem acesso à variável "nome"  da função externa
     }
    
      return getNome;   // Retorna a função interna, expondo-a assim para escopos externos
      //**Porem só expoe o que ela retorna de resultado e não o que foi declarado dentro dela 
    },
    umaPessoa = pessoa("Christy");
    
    umaPessoa();// Retorna "Christy"


**Se eu colocasse uma variável na função interna, por exemplo, não conseguiria chamar ela, só o resultado que a função retorna.