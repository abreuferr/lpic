# 351 Virtualização completa

## Resultados esperados

Explique hypervisors tipo 1 e 2, VM monitor, emulação, paravirtualização,
hardware assistido, snapshots, migração e os papéis de QEMU, KVM, Xen e
libvirt. Pratique o ciclo de vida de uma VM, armazenamento e redes virtuais.

## Laboratório

```bash
virt-host-validate
virsh list --all
virsh net-list --all
qemu-img info imagem.qcow2
```

Crie uma VM descartável, associe uma interface à rede virtual, faça um snapshot
e restaure-o. Documente a diferença entre snapshot de disco e snapshot que
inclui estado de memória.

## Material reutilizável

- `../../304/doc/330_3_kvm.txt`
- `../../304/doc/330_5_libvirt_and_related_tools.txt`
