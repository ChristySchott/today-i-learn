### Acessando variáveis de outro formulário

Ao fazer um projeto eu crio dois Forms: o Unit1 e o Unit2. Programando no Unit2, decido pegar uma variável que utilizei no primeiro Form. O que devo fazer?

Tenho que importar o Unit1, e para fazer isso eu abr o Unit2 e aperto ***alt+F11***. 

1. Selecione o Form desejado e clique no botão *OK*;
2. O Form será importado em baixo do valor *Implementation*, no nosso caso estamos importando o Unit1 então código ficará assim:

    `Implementation`
	
	 `uses Unit1;`

3. Agora  basta chamar o nome do Form importado mais um '.' e então o nome da variável que desejo importar:

			`begin

			NomeForm.nomevariavel

			end;`

### Obs:
Só posso importar variáveis declaradas como públicas, as privadas são de exclusividade do formulário. 