# 352 Virtualização por containers

## Conceitos

Containers de sistema e de aplicação compartilham o kernel do host. Entenda
namespaces, cgroups, capabilities, seccomp, SELinux/AppArmor, OCI, runc,
containerd, CRI-O, Docker, LXC, Podman, Buildah e Skopeo.

## Laboratório rootless

```bash
podman run --rm docker.io/library/alpine:latest uname -a
podman ps --all
podman inspect --format '{{.State.Pid}}' CONTAINER
lsns -p PID
```

Substitua `CONTAINER` e `PID` pelos valores locais. Compare namespaces e
cgroup do processo com os do host. Não use `--privileged` para resolver erros:
identifique primeiro qual permissão, volume, porta ou política está ausente.

## Revisão

Explique a diferença entre imagem, container, volume e registry; entre rootful
e rootless; e entre o runtime OCI e o runtime de alto nível.
