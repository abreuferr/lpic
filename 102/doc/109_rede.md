# 109 Fundamentos de rede

## Objetivos 109.1 a 109.4

Cubra IPv4/IPv6, CIDR, rota padrão, TCP/UDP, DNS do cliente e configuração
persistente de interfaces.

## Comandos essenciais

```bash
ip addr show
ip route show
ip -6 route show
ss -tulpn
ping -c 3 endereco
dig exemplo.org
resolvectl status
```

Estude também `/etc/hosts`, `/etc/resolv.conf`, `/etc/nsswitch.conf` e o
gerenciador de rede da distribuição, como NetworkManager com `nmcli`.

## Exercício de diagnóstico

Com uma VM sem acesso à rede, verifique nesta ordem: link e endereço, rota,
alcance do gateway, resolução de nome e porta do serviço. Registre qual comando
comprova cada hipótese.
