# LPIC-3 305-300: Virtualization and Containerization

Este diretório é a trilha atual que substitui a parte de virtualização do
304-200. As notas de KVM e libvirt em `../304/doc/` são pré-requisitos úteis,
mas não cobrem containers nem provisionamento moderno.

| Tópico | Estado | Roteiro |
| --- | --- | --- |
| 351 Full Virtualization | Parcial | `doc/351_virtualizacao_completa.md` e notas históricas de KVM/libvirt |
| 352 Container Virtualization | Inicial | `doc/352_containers.md` |
| 353 VM Deployment and Provisioning | Inicial | `doc/353_provisionamento.md` |

## Ambiente sugerido

Use uma máquina Linux com virtualização aninhada quando necessária. Para
containers, prefira Podman rootless em uma VM descartável. Mantenha imagens,
volumes e redes de laboratório separados do ambiente pessoal.

## Referência oficial

- https://wiki.lpi.org/wiki/LPIC-305_Objectives_V3.0
