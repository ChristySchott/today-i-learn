
# Loaders

Os **Loaders** permitem que os arquivos sejam pré-processados ​​como e quando precisam ser carregados.

Eles fornecem uma maneira poderosa de lidar com as etapas de criação do front-end e geralmente são usados para transformar arquivos de uma linguagem diferente ou para requisitá-los.

Para não especificar **loaders** em cada módulo únicos, pode-se usar a seguinte configuração:

```
{ 
  module: { 
    loaders: [
      {test: /\.jade$/, loader: "jade"},
      {test: /\.css$/, loader: "style!css"},
      {test: /\.coffee$/, loader: "coffee-loader"}
    ]
  }
}
```



<!--stackedit_data:
eyJoaXN0b3J5IjpbLTUzOTQyMjc1Ml19
-->