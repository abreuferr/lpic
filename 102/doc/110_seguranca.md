# 110 Segurança

## Objetivos 110.1 a 110.4

Estude permissões, contas, PAM, sudo, SSH, GPG, hashes e integridade de
arquivos. A meta é compreender controles de acesso e aplicar o menor privilégio.

## Checklist

- Comparar permissões tradicionais, `umask`, SUID/SGID e sticky bit.
- Usar `visudo`, grupos administrativos e `sudo -l`.
- Configurar chaves SSH e permissões de `~/.ssh`.
- Criar, verificar e revogar assinaturas GPG em material de laboratório.
- Verificar pacotes instalados com as ferramentas da distribuição.

## Exercício

Crie uma chave SSH para um usuário de laboratório, restrinja as permissões de
`~/.ssh`, teste a autenticação e explique por que uma chave privada jamais deve
ser colocada em um repositório real. A nota `sudo.txt` é uma referência
histórica de uso, não um modelo para publicar hashes de contas.
