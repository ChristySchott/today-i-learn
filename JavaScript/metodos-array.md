# Methods

## push()

O método push adiciona um valor a um array.

~~~
  var fruits = ["Banana", "Orange", "Apple", "Mango"];

 function myFunction() {

  fruits.push("Kiwi");
  
  document.getElementById("demo").innerHTML = fruits;
  
 }
 ~~~
 
 Aqui eu adicionei o Kiwi na lista de frutas.
 
 ## pop()

O método pop remove o ultimo valor de um array.

~~~
  var fruits = ["Banana", "Orange", "Apple", "Mango"];

 function myFunction() {

  fruits.pop("Mango");
  
  document.getElementById("demo").innerHTML = fruits;
  
 }
 ~~~
 
 Aqui eu removi a manga na lista de frutas.
 
 ## Push()

O método push adiciona um valor a um array.

~~~
  var fruits = ["Banana", "Orange", "Apple", "Mango"];

 function myFunction() {

  fruits.push("Kiwi");
  
  document.getElementById("demo").innerHTML = fruits;
  
 }
 ~~~
 
 Aqui eu adicionei o Kiwi na lista de frutas.
 
 ## join()

O método join adiciona um array a uma string

~~~
  var fruits = ["Banana", "Orange", "Apple", "Mango"];

 function myFunction() {

  fruits.join("*");
  
  document.getElementById("demo").innerHTML = fruits;
  
 }
 ~~~
 
 Aqui eu adicionei o * entra os elementos na lista de frutas.
 Resultado: "Banana * "Orange * "Apple * Mango"
 
 ## concat()

O método concat me permite concatenar duas arrays.

~~~
  var frutas1 = ["Banana", "Orange"];
var frutas2 = ["Apple", "Mango"];
var frutasTotal = frutas1.concat(frutas2);
  
 }
 ~~~
 
 Aqui eu juntei os dois.
 Resultado: "Banana,Orange,Apple,Mango"
 
 
  ## splice()

O método splice me permite adicionar valores a determinadas posições do array

~~~
  var fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo1").innerHTML = "Original Array:<br>" + fruits;
function myFunction() {
  fruits.splice(2, 0, "Lemon", "Kiwi");
  document.getElementById("demo2").innerHTML = "New Array:<br>" + fruits;
  
 }
 ~~~
 
 Aqui eu adicionei o Lemon na posição de index 2 e o Kiwi logo após.
 Resultado: "Banana,Orange,Lemon,Kiwi,Apple,Mango"
