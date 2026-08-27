# 364 HA em nó único

Mesmo sem cluster, disponibilidade depende de prevenção e recuperação:
SMART/NVMe, UPS, monit, RAID avançado, LVM avançado, bonding, VLANs e noções de
BGP para links redundantes.

## Laboratório seguro

```bash
smartctl -a /dev/sdX
cat /proc/mdstat
lvs -a -o +devices
ip -d link show
```

Use discos virtuais descartáveis para simular falha de RAID e recuperação. Para
rede, crie interfaces virtuais ou uma topologia de VMs; não altere bonding ou
VLAN da interface que mantém sua conexão administrativa.
