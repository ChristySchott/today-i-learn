
# Date()

Para pegar a data atual basta apenas usar o comando "Date()", como no exemplo abaixo:


<button type="button
onclick="document.getElementById('aqui').innerHTML = Date()">*<*button*>*

*<*p id="aqui"></p*>*

No HTML da página eu criei um botão e um parágrafo para onde enviarei o meu resultado. O código funcionará da seguinte maneira: 
1. O evento *onclick* avisa o programa que será feito algo quando o button for clicado.
2. Pego o id *aqui* pelo comando *getElementById()*.
3. Aviso que ele será colocado no arquivo HTML com o *innerHTML*.
4. Atribui um valor para ele, que será o Date()
5. O date automaticamente pega a hora e a data atual.
6. O resultado é passado para a id que enviei, no caso ela está no paragrafo.

O resultado será o seguinte:

Sat Mar 28 2020 09:24:15 GMT-0300 (Horário Padrão de Brasília)
