# 105.2 Shell scripting

## Objetivo

Criar scripts POSIX simples, tratar argumentos, fluxo de controle, códigos de
saída e expansão de comandos.

## Checklist

- Shebang, permissões de execução e execução com `sh script.sh`.
- Parâmetros: `$0`, `$1`, `$#`, `$@`, `shift` e `getopts`.
- Testes com `test`, `[ ]`, `case`, `if`, `for`, `while` e `until`.
- Substituição de comando `$(comando)`, redirecionamentos e códigos de saída.
- Quoting: use aspas duplas para expandir variáveis; use aspas simples para
  texto literal; sempre proteja caminhos com espaços.

## Laboratório

```sh
#!/bin/sh
set -eu

usage() { printf 'uso: %s DIRETORIO\n' "$0" >&2; exit 2; }
[ "$#" -eq 1 ] || usage
[ -d "$1" ] || { printf 'diretorio inexistente\n' >&2; exit 1; }

find "$1" -type f -print | wc -l
```

Teste os casos de sucesso, argumento ausente e diretório inexistente. Execute
`shellcheck` quando disponível, mas não dependa dele para a prova.
