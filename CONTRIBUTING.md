# Como contribuir

Vale para todos os repositórios da organização que não tenham guia próprio.

## Fluxo

1. Toda mudança começa por uma issue, aberta pelos formulários (bug, funcionalidade, demanda com spec, infraestrutura, achado de auditoria).
2. Crie a branch a partir da `main` atualizada.
3. Abra a pull request para a `main`, preenchendo o template e a barra lateral.
4. A `main` é a única fonte da verdade. Ambientes como homologação recebem a mudança para teste, mas nunca são promovidos de volta para a `main`.
5. Merge só com revisão aprovada e, quando o repositório tiver CI, com a verificação verde.

## Nomes de branch

| Prefixo | Uso |
|---|---|
| `feature/` | Funcionalidade nova |
| `fix/` | Correção de bug |
| `refactor/` | Refatoração sem mudar comportamento |
| `test/` | Testes |
| `docs/` | Documentação |
| `chore/` | Manutenção e dependências |
| `ci/` | CI/CD |

Use letras minúsculas e hífens: `fix/duplicidade-etiquetas`.

## Commits

[Conventional Commits](https://www.conventionalcommits.org): `<tipo>(<escopo opcional>): <descrição>`, com descrição no imperativo e em português.

Tipos: `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, `build`, `ci`, `chore`, `revert`.

## O que não entra no Git

- `.env`, chaves, tokens, certificados, bancos de dados, dumps, logs e arquivos compactados. Veja a [política de segurança](SECURITY.md).
- Documentos de processo: planos, evidências de investigação, handoffs. Eles ficam fora do repositório. Decisões duráveis viram ADR (`docs/adr/`), procedimentos viram runbook (`docs/runbooks/`) e termos do domínio vão para o `GLOSSARY.md`.

## Prova antes de "pronto"

Uma mudança só está concluída quando o comando de teste ou verificação foi executado e a saída está na PR. Achado de investigação só é registrado depois de reproduzido.

## Conduta

Veja o [código de conduta](CODE_OF_CONDUCT.md).
