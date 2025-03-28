# Como *Escapar Código*?
É bem simples escapar códigos no bdfd, eles servem para que não seja executado no código, mas apenas executado dentro de um `$eval`.
- \ › \\\
- $ › %{DOL}% `($$c[] também serve se preferir)`
- ; › \;
- ] › \\]

## Exemplos
`%{DOL}%username` › Retorna: $username

`$eval[%{DOL}%username]` › Retorna: btw.sean

> Em breve terá um conversor para isso.
