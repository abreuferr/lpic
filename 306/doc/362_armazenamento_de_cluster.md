# 362 Armazenamento de cluster

Estude SAN, Fibre Channel, iSCSI, multipath, DLM, clustered LVM, GFS2 e OCFS2.
O ponto central é entender quem possui o lock e quais nós podem montar um
filesystem compartilhado com segurança.

## Checklist de laboratório

```bash
iscsiadm -m session
multipath -ll
pvs
vgs
lvs
```

Antes de criar um filesystem de cluster, confirme a topologia de blocos, os
paths redundantes e a camada de locking. Nunca monte um filesystem comum em
modo escrita em múltiplos nós como se fosse compartilhado.
