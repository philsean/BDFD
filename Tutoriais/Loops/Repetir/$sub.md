# Loop com $sub ( Recomendado )
O conceito básico deste loop é repetir o código **y vezes**, sendo assim possivelmente um loop de quantas vezes você quiser. O `$sub[1eY;1]` vai criar uma sequência de 9 de acordo com Y, exemplo: `1e5` › 99999, posteriormente o $replaceText vai substituir tudo isso pelo seu código.

- Código sem retorno:
```js
$async[code]
$c[ Código Escapado, siga em frente para saber como fazer | Exemplo: ]
%{DOL}%var[text\;%{DOL}%var[text\]a\]
$endasync
$var[y;5] $c[ Quantas vezes vai repetir ]
$eval[$replaceText[$sub[1e$var[y];1];9;$await[code]]]
```
- Código com retorno
```js
$var[y;5] $c[ Quantas vezes vai repetir ]
$var[code;Exemplo] $c[ Código Escapado ]
$eval[$replaceText[$sub[1e$var[y];1];9;$var[code]]]
```

> Caso você não saiba escapar código clique aqui: [como escapar]()
