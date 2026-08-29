# Projeto: lpic

Repositório pessoal de anotações de estudo para LPIC-1/2/3 (não é um projeto de software). Antes de propor mudanças estruturais, entenda que o valor está no conteúdo das notas, não em código. Ver README.md para estrutura de diretórios, convenção de nomes de arquivo, licença e autor.

## Convenções do repositório

- Existem dois estilos de nota, ambos válidos — não normalizar um para o outro sem pedido explícito:
  - **Transcrição de terminal** (maioria em `101/`, `102/`, parte de `201/`): comandos com saída real, sem cabeçalho formal.
  - **Objetivo LPI formal** (maioria em `202/`, `303/`, `304/`): cabeçalho `#: Title / #: Author / #: Description / #: Options: Weight: N`, seguido da descrição oficial do objetivo e "Key Knowledge Areas". Os arquivos `.md` mais recentes em `202/doc/` (ex. `207_2_dns.md`) são o formato mais atual: markdown estruturado com seções, referências externas e exemplos — preferir esse formato ao criar notas novas.
- Notas em português do Brasil (pt-BR); comandos e configs mantidos no idioma original de origem.

## Atenção

- `303/src/` e `303/src/certs/` contêm chaves privadas, CSRs, certificados e uma passphrase **já commitados no histórico do git** — são material de laboratório (PKI de estudo para o objetivo 325), não segredos de produção. Não tratar como incidente de segurança a corrigir automaticamente; se for necessário sanitizar o histórico, confirmar com o usuário antes (reescrever histórico é destrutivo).
- Remote: `git@github.com:abreuferr/lpic.git`. Sem instrução permanente de push para este projeto — tratar como qualquer repositório: nunca fazer `git push` sem confirmação explícita do usuário na mensagem atual.
