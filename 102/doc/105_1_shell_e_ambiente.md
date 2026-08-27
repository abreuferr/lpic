# 105.1 Shell e ambiente

## Objetivo

Usar e personalizar o shell, perfis de login, variáveis de ambiente, aliases,
funções e histórico de comandos.

## Pontos de estudo

- Arquivos de inicialização: `/etc/profile`, `/etc/bash.bashrc`, `~/.profile`,
  `~/.bash_profile` e `~/.bashrc`.
- Diferença entre shell de login e shell interativo.
- Variáveis locais, exportadas e somente leitura: `NAME=value`, `export NAME`,
  `readonly NAME`, `unset NAME`.
- `PATH`, `PS1`, `HOME`, `LANG`, `EDITOR`, `umask`, `alias`, `unalias`,
  `type`, `which` e `history`.

## Laboratório

```bash
mkdir -p ~/lpic-102-lab/bin
printf '%s\n' '#!/bin/sh' 'printf "ola %s\\n" "$USER"' > ~/lpic-102-lab/bin/ola
chmod 755 ~/lpic-102-lab/bin/ola
PATH="$HOME/lpic-102-lab/bin:$PATH"
export PATH
type ola
ola
alias ll='ls -lah'
```

Valide em um novo shell que alterações temporárias não persistem. Depois,
adicione somente a configuração desejada ao arquivo de inicialização adequado.

Veja também: `variavel.txt` e `expressao_regular.txt`.
