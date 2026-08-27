# LPIC

Anotações pessoais de estudo para as certificações **LPIC-1, LPIC-2 e LPIC-3** (Linux Professional Institute Certification), organizadas por exame/tópico oficial do LPI.

## Estrutura

Cada diretório numerado corresponde a um exame da grade LPI:

| Diretório | Exame                  | Certificação |
|-----------|-------------------------|--------------|
| `101`     | Exam 101                | LPIC-1       |
| `102`     | Exam 102                | LPIC-1       |
| `201`     | Exam 201                | LPIC-2       |
| `202`     | Exam 202                | LPIC-2       |
| `303`     | Exam 303 (Security)      | LPIC-3       |
| `304`     | Exam 304 (Virtualization & HA, aposentado) | Referência histórica |
| `305`     | Exam 305 (Virtualization & Containerization) | LPIC-3 |
| `306`     | Exam 306 (High Availability & Storage Clusters) | LPIC-3 |

Dentro de cada exame:

- `doc/` — anotações de estudo (comandos, teoria, objetivos do exame).
- `src/` — arquivos de apoio usados nos exercícios práticos (configs, scripts, chaves/certificados de laboratório, LDIFs etc.), quando aplicável.

Os arquivos de `doc/` seguem o padrão `<tópico>_<subtópico>_<assunto>.txt` (ex.: `207_2_dns.md` = tópico 207, subtópico 2, DNS), com base na numeração oficial dos objetivos do LPI.

## Como estudar

Cada diretório de exame possui um `INDEX.md` que relaciona os objetivos da prova
com as notas e laboratórios locais. Os índices distinguem material completo,
parcial e pendente; eles são o ponto de partida para uma revisão orientada à
versão atual da prova.

Os diretórios `304/` e `303/` preservam material de versões anteriores. Para
certificação atual, use respectivamente `305/` e `306/`, e o mapa de migração
em `303/INDEX.md`.

## Licença

Conteúdo dedicado ao domínio público sob [CC0 1.0 Universal](LICENSE).

## Autor

Caio Abreu Ferreira
