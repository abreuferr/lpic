# 353 Implantação e provisionamento de VMs

## Escopo

Estude conceitos de IaaS, PaaS, SaaS, OpenStack, Terraform, Packer, cloud-init
e Vagrant. O objetivo é produzir máquinas repetíveis, não criar servidores
manualmente a cada laboratório.

## Sequência prática

1. Crie uma imagem base sem credenciais embutidas.
2. Use Packer para produzir a imagem, quando disponível.
3. Use cloud-init para criar usuário, chave SSH, hostname, pacotes e discos.
4. Use Terraform ou Vagrant para declarar e criar a instância.
5. Valide conectividade, armazenamento, inventário e destruição do ambiente.

## Exemplo de user-data

```yaml
#cloud-config
users:
  - name: aluno
    groups: [sudo]
    sudo: ALL=(ALL) NOPASSWD:ALL
    ssh_authorized_keys:
      - ssh-ed25519 CHAVE_PUBLICA_DE_LABORATORIO
package_update: true
packages: [curl]
```

Use somente chave pública de laboratório. A credencial privada correspondente
não deve entrar na imagem nem no repositório.
