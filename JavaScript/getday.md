# getDay()

Usando a função getDay eu posso pegar tanto o número do dia como o nome dele.

##### Pegando o número:

var d = new Date();

document.getElementById("demo").innerHTML = d.getDay();

##### Pegando o nome (coloco ele num array):

var d = new Date();

var days = ["Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday"];

document.getElementById("demo").innerHTML = days[d.getDay()];
