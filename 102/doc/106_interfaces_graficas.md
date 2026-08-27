# 106 Interfaces gráficas

## Objetivos 106.1 a 106.3

Estude a arquitetura do X11, acesso remoto, ambientes de desktop e
acessibilidade. A prova cobra conceitos e arquivos de configuração, não a
preferência por um desktop específico.

## Checklist prático

- Identificar `DISPLAY`, `XAUTHORITY`, `xhost`, `xauth` e `ssh -X`/`ssh -Y`.
- Distinguir display manager, window manager e desktop environment.
- Reconhecer `~/.xinitrc`, `~/.Xresources` e arquivos em `/etc/X11/`.
- Configurar idioma, teclado e opções básicas de acessibilidade pela sessão
  gráfica e entender o impacto de `LANG` e `LC_*`.

## Exercício

Em uma VM com X11, conecte-se com `ssh -X`, confirme `echo "$DISPLAY"` e
execute uma aplicação gráfica simples. Em seguida, explique por que `xhost +`
não é uma configuração aceitável em uma máquina compartilhada.
