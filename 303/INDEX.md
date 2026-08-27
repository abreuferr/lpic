# LPIC-3 Security 303-300

O diretório `303/` começou com notas da versão 2.0, identificadas pelos
tópicos `325` a `328`. A prova atual é a 303-300, versão 3.0, identificada
pelos tópicos `331` a `335`. As notas antigas continuam úteis, mas este mapa
deixa explícito o que pode ser reutilizado e o que precisa ser estudado além
delas.

| Objetivo atual | Cobertura local | Ação de estudo |
| --- | --- | --- |
| 331.1 PKI e X.509 | Parcial | Usar `325_1`; acrescentar certificate transparency, ACME, certbot e CFSSL. |
| 331.2 TLS e autenticação X.509 | Parcial | Usar `325_2`; revisar Apache 2.4, SNI, HSTS e OCSP stapling. |
| 331.3 Sistemas de arquivos cifrados | Parcial | Usar `325_3`; acrescentar LUKS2 e Clevis/Tang. |
| 331.4 DNS e criptografia | Parcial | Usar `325_4`; acrescentar DoT, DoH e mDNS. |
| 332.1 Hardening de host | Parcial | Usar `326_1`; acrescentar USBGuard, certificados SSH e sandboxing systemd. |
| 332.2 Detecção de intrusão de host | Parcial | Usar `326_2`; praticar auditd, AIDE e verificação de pacotes. |
| 332.3 Controle de recursos | Pendente | Estudar ulimits, cgroups v2, slices, scopes e `systemd-cgtop`. |
| 333.1 DAC | Parcial | Usar `327_1` e `333_1`; revisar atributos estendidos. |
| 333.2 MAC | Parcial | Usar `327_2` e `334_1`; priorizar SELinux, mantendo AppArmor como awareness. |
| 334.1 Hardening de rede | Parcial | Usar `328_1`; reforçar segmentação e validação de controles. |
| 334.2 Detecção de intrusão de rede | Parcial | Usar `328_2`; complementar com ferramentas atuais. |
| 334.3 Filtragem de pacotes | Parcial | Usar `328_3`; praticar nftables. |
| 334.4 VPN | Parcial | Usar `328_4`; acrescentar strongSwan, IKEv2 e WireGuard. |
| 335.1 Ameaças e vulnerabilidades | Pendente | Criar resumos de ameaças, mitigação e honeypots. |
| 335.2 Teste de intrusão | Pendente | Estudar escopo legal, fases do teste e Nmap Scripting Engine. |

## Material que mudou de especialidade

`326_3_user_management_and_authentication.txt` e
`326_4_freeipa_installation_and_samba_integration.txt` são material valioso,
mas não pertencem mais ao 303-300. Eles se alinham à especialização LPIC-3
Mixed Environments 300-300, sobretudo a identidade Linux e FreeIPA.

## Ordem recomendada

1. Atualize os quatro objetivos 331, pois as notas existentes já dão a base.
2. Faça laboratórios controlados para 332 e 333 antes de qualquer varredura de
   rede.
3. Estude 334 e 335 somente em ambientes próprios ou explicitamente
   autorizados.

## Referência oficial

- https://www.lpi.org/our-certifications/exam-303-objectives/
