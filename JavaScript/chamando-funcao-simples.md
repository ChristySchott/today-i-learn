# Chamando funções



Apenas definir uma função não faz com que ela seja executada, simplesmente a nomeia e especifica o que fazer quando ela for chamada. Para executar as ações indicadas no parâmetro da função, ela deve ser chamada. Ao definir uma função, você pode chamá-la do seguinte modo: 


> funcao(5);
 
Não importa se essa declaração for chamada antes da função, desde que elas estejam na mesma página. Por exemplo:

    Aqui a função é chamada: funcao();


	Aqui ela é declarada:  function funcao() {
						return (x+x) 
						};


####Importante:
Ela só pode ser chamada antes se for declarada daquele jeito, deste outro modo não funcionaria:

        console.log(square(5));
    	var square = function (n) {
      	return n * n;
   		}


Claro que há outros modos de chamar uma função, mas coloquei o mais simples pois este Markdown é destinado a iniciantes na linguagem.