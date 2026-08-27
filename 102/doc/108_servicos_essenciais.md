# 108 Serviços essenciais

## Objetivos 108.1 a 108.4

### Tempo e logs

Pratique `timedatectl`, `chronyc`, `journalctl`, `logger`, `systemctl status`
e filtros por unidade, prioridade e intervalo de tempo. Reconheça rsyslog e os
arquivos tradicionais em `/var/log`.

### Correio e impressão

Entenda o papel do MTA, aliases, fila de mensagens e encaminhamento local.
Para impressão, saiba identificar CUPS, `lp`, `lpr`, `lpstat` e filas.

## Exercício

Gere uma entrada com `logger -p user.notice "teste lpic"`, localize-a com
`journalctl` e identifique qual processo mantém uma porta aberta usando
`ss -lntp` ou `fuser`. Veja `log.txt` e `fuser.txt`.
