# Eventos para manipular vídeos adicionados na página

- ### Adicionando vídeo no HTML

Caso não saiba como adicionar um vídeo a sua página aqui tem um exemplo da sintaxe usada no documento HTML de um site:

> <video src="nome-do-video.mp4"  width:"100%" controls="controls"> </video>

Vale dizer que sem o recurso "controls" o vídeo apareceria na tela sem os controles de navegação e a barra do tempo exibida embaixo da tela.

Para manipular o vídeo no JS irei adicionar uma classe no vídeo:

> <video **class="video" src="nome-do-video.mp4"  width:"100%" controls="controls"> </video>

- ### Manipulando vídeo no JavaScript

Agora no documento .js eu crio uma varial e atribuo a ela o vídeo:

> var pegando = document.querySelector('.video');

*Repare que estamos pegando o video através de sua classe, por isso atribuimos uma classe a ele no HTML*

Agora eu adiciono o evento:

> pegando.*addEventListener*("play", function(){
>   alert("Apertou o play");
> }

No exemplo acima eu defini que algo acontecesse caso o evento *PLAY* fosse "ativado". Existem ainda outros eventos como o *ended*:

> > pegando.*addEventListener*("ended", function(){
>   alert("Acabou o vídeo");
> }

Nesse caso quando o video acabar será mostrado o alerta. Existe também o *seeking*:

> pegando.*addEventListener*("seeking", function(){
>   alert("Você está em: " +  this.currentTime(););
> }

Seeking vai ser ativado quando eu clicar em algum momento do vídeo na barra de progresso. Usei o comando *this.currentTime* para informar o tempo exato que eu cliquei.

