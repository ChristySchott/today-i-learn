---


---

<h1 id="usando-mixin-no-sass">Usando Mixin no SASS</h1>
<p>Sendo um recurso da ferramenta SASS, o Mixin facilita muito a elaboração de um sintaxe mais légivel e reduzida do CSS.</p>
<h2 id="vantagens">Vantagens</h2>
<p>O SASS é uma linguagem que extende o CSS que facilita o dia-a-dia do programador web e é essencial hoje em dia</p>
<p>no desenvolvimento front-end.</p>
<p>Mixins permitem que você reutilize o código sem ter que adicionar classes no seu HTML e principal vantagem</p>
<p>de utilizar @mixin é que eles podem receber variáveis.</p>
<h3 id="exemplos">Exemplos</h3>
<p>A seguir exemplos da utilização de mixins em código CSS.</p>
<pre><code>
@mixin mixins-sao-demais($radius: 20px) {

border-radius: $radius;

}

Você pode usar ele como propriedade:

/* Utilizando o valor padrão para o argumento. */

.classe1 {

@include mixins-sao-demais;

}

/* Passando um valor próprio como argumento. */

.classe2 {

@include mixin-sao-demais(10px);

}

</code></pre>
<h3 id="principais-mixins">Principais Mixins</h3>
<p>Mais alguns exemplos de mixins que facilitarão sua vida.</p>
<pre><code>
Para centralizar:

@mixin push--auto {

margin: {

left: auto;

right: auto;

}

}

Fontes:

@mixin font-source-sans($size: false, $colour: false, $weight: false, $lh: false) {

font-family: 'Source Sans Pro', Helvetica, Arial, sans-serif;

@if $size { font-size: $size; }

@if $colour { color: $colour; }

@if $weight { font-weight: $weight; }

@if $lh { line-height: $lh; }

}

Uso do before e after (pseudo-elementos):

@mixin pseudo($display: block, $pos: absolute, $content: ''){

content: $content;

display: $display;

position: $pos;

}

</code></pre>
<pre><code></code></pre>
<p>Um esquema de aprendizado:<br>
<strong>Lembrando que antes de estudar algum framework, domine o JS</strong></p>
<div class="mermaid"><svg xmlns="http://www.w3.org/2000/svg" id="mermaid-svg-zeJU5pKQrAYJj1ZM" width="100%" style="max-width: 606.1000061035156px;" viewBox="0 0 606.1000061035156 184"><g transform="translate(-12, -12)"><g class="output"><g class="clusters"></g><g class="edgePaths"><g class="edgePath" style="opacity: 1;"><path class="path" d="M121.72535211267606,81L225.5,33L331.5,49.145695364238414" marker-end="url(#arrowhead3489)" style="fill:none"></path><defs><marker id="arrowhead3489" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker></defs></g><g class="edgePath" style="opacity: 1;"><path class="path" d="M124,111.7915309446254L225.5,127L327,143.8046357615894" marker-end="url(#arrowhead3490)" style="fill:none"></path><defs><marker id="arrowhead3490" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker></defs></g><g class="edgePath" style="opacity: 1;"><path class="path" d="M421.5,43.919463087248324L451,36L504.9873467020851,76.012650246157" marker-end="url(#arrowhead3491)" style="fill:none"></path><defs><marker id="arrowhead3491" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker></defs></g><g class="edgePath" style="opacity: 1;"><path class="path" d="M406.0431034482759,129L451,94L483.07030602207044,97.92969092617184" marker-end="url(#arrowhead3492)" style="fill:none"></path><defs><marker id="arrowhead3492" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker></defs></g><g class="edgePath" style="opacity: 1;"><path class="path" d="M124,96.2084690553746L225.5,81L331.5,63.450331125827816" marker-end="url(#arrowhead3493)" style="fill:none"></path><defs><marker id="arrowhead3493" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker></defs></g><g class="edgePath" style="opacity: 1;"><path class="path" d="M121.72535211267606,127L225.5,175L327,159.53973509933775" marker-end="url(#arrowhead3494)" style="fill:none"></path><defs><marker id="arrowhead3494" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker></defs></g><g class="edgePath" style="opacity: 1;"><path class="path" d="M406.0431034482759,79L451,114L483.0703115274953,111.07030847573749" marker-end="url(#arrowhead3495)" style="fill:none"></path><defs><marker id="arrowhead3495" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker></defs></g><g class="edgePath" style="opacity: 1;"><path class="path" d="M426,165.28859060402684L451,172L504.987350212417,132.98734716065934" marker-end="url(#arrowhead3496)" style="fill:none"></path><defs><marker id="arrowhead3496" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"></path></marker></defs></g></g><g class="edgeLabels"><g class="edgeLabel" transform="translate(225.5,33)" style="opacity: 1;"><g transform="translate(-24,-13)" class="label"><foreignObject width="48" height="26"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel">Leitura</span></div></foreignObject></g></g><g class="edgeLabel" transform="translate(225.5,127)" style="opacity: 1;"><g transform="translate(-76.5,-13)" class="label"><foreignObject width="153" height="26"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel">Curva de aprendizado</span></div></foreignObject></g></g><g class="edgeLabel" transform="" style="opacity: 1;"><g transform="translate(0,0)" class="label"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel" transform="" style="opacity: 1;"><g transform="translate(0,0)" class="label"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel" transform="translate(225.5,81)" style="opacity: 1;"><g transform="translate(-24.5,-13)" class="label"><foreignObject width="49" height="26"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel">Cursos</span></div></foreignObject></g></g><g class="edgeLabel" transform="translate(225.5,175)" style="opacity: 1;"><g transform="translate(-74,-13)" class="label"><foreignObject width="148" height="26"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel">Pesquisa de mercado</span></div></foreignObject></g></g><g class="edgeLabel" transform="" style="opacity: 1;"><g transform="translate(0,0)" class="label"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel" transform="" style="opacity: 1;"><g transform="translate(0,0)" class="label"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span class="edgeLabel"></span></div></foreignObject></g></g></g><g class="nodes"><g class="node" id="A" transform="translate(72,104)" style="opacity: 1;"><rect rx="0" ry="0" x="-52" y="-23" width="104" height="46"></rect><g class="label" transform="translate(0,0)"><g transform="translate(-42,-13)"><foreignObject width="84" height="26"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;">Square Rect</div></foreignObject></g></g></g><g class="node" id="B" transform="translate(376.5,56)" style="opacity: 1;"><rect rx="5" ry="5" x="-45" y="-23" width="90" height="46"></rect><g class="label" transform="translate(0,0)"><g transform="translate(-35,-13)"><foreignObject width="70" height="26"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;">Prática JS</div></foreignObject></g></g></g><g class="node" id="C" transform="translate(376.5,152)" style="opacity: 1;"><rect rx="5" ry="5" x="-49.5" y="-23" width="99" height="46"></rect><g class="label" transform="translate(0,0)"><g transform="translate(-39.5,-13)"><foreignObject width="79" height="26"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;">Framework</div></foreignObject></g></g></g><g class="node" id="D" transform="translate(543.0500030517578,104)" style="opacity: 1;"><polygon points="67.05,0 134.1,-67.05 67.05,-134.1 0,-67.05" rx="5" ry="5" transform="translate(-67.05,67.05)"></polygon><g class="label" transform="translate(0,0)"><g transform="translate(-41.5,-13)"><foreignObject width="83" height="26"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;">Proficiência</div></foreignObject></g></g></g></g></g></g></svg></div>

