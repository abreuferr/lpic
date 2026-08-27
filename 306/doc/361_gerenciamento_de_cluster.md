# 361 Gerenciamento de clusters HA

## Conceitos essenciais

Compare active/passive, active/active, failover, balanceamento, shared-nothing,
shared-disk, quorum, fencing, split brain, RTO, RPO, MTBF e MTTR. Toda decisão
de HA precisa declarar o que acontece quando um nó, uma rede ou o storage falha.

## Laboratório de balanceamento

Com duas VMs backend e uma VM de balanceamento, configure health checks e uma
VIP usando HAProxy e keepalived. Pare um backend e confirme que o tráfego deixa
de ser enviado a ele. Depois pare o nó ativo e verifique o failover da VIP.

Registre os comandos de validação, o tempo de detecção e o comportamento de
sessões ativas. Não teste failover em infraestrutura fora do laboratório.
