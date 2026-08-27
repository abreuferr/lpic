# 332.3 Controle de recursos

## Objetivo

Restringir o consumo de recursos por serviços e processos usando ulimits,
cgroups e recursos do systemd.

## Conceitos

- `ulimit` aplica limites ao shell e aos processos descendentes; limites
  persistentes para sessões usam `/etc/security/limits.conf` e PAM.
- Cgroups agrupam processos para contabilizar e limitar CPU, memória, I/O e
  número de processos.
- No systemd, services, scopes e slices organizam cgroups. Uma unidade pode
  receber `MemoryMax=`, `CPUQuota=`, `TasksMax=` e `IOWeight=`.

## Laboratório

```bash
systemd-cgls
systemd-cgtop
systemctl show ssh.service -p MemoryCurrent -p TasksCurrent
systemd-run --user --scope -p MemoryMax=256M sleep 30
```

Em uma VM, crie um override para um serviço não crítico com `systemctl edit`.
Valide a sintaxe, reinicie o serviço e confirme o limite com `systemctl show`.
Nunca imponha limites desconhecidos em serviços de produção.
