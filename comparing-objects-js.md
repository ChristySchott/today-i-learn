
Não existe uma forma direta de comparar objetos no JS, mas você pode chegar comparando as propriedades.

**var comparando = function(a, b) { if (Object.keys(a).length !== Object.keys(b).length) { return false; }**

  for (var i in a) {
    if (a[i] !== b[i]) { return false; }
  }
  return true;
};

O  `Object.keys(a).length`  talvez não funcione em browsers antigos.


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4NDE5MzY1NDldfQ==
-->