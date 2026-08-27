# 107 Tarefas administrativas

## Objetivos 107.1 a 107.3

### Contas e grupos

Pratique `useradd`, `usermod`, `userdel`, `groupadd`, `groupmod`, `passwd`,
`chage`, `id`, `getent` e os arquivos `/etc/passwd`, `/etc/shadow`,
`/etc/group` e `/etc/skel`. Prefira `visudo` para editar regras do sudo.

### Agendamento

Compare `cron`, `at`, `systemd timers` e `anacron`. Verifique o serviço,
permissões e logs antes de diagnosticar uma tarefa que não executou.

```bash
systemctl list-timers --all
crontab -l
atq
```

### Localização

Use `locale`, `localectl`, `timedatectl` e `tzselect`. Diferencie locale,
fuso horário e layout de teclado.

## Exercício

Crie um usuário de laboratório com expiração, um grupo suplementar e uma tarefa
agendada que escreva data e hora em um arquivo no diretório do usuário. Remova
tudo ao final. Veja também `at.txt` e `sudo.txt`.
