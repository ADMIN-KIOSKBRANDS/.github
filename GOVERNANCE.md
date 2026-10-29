# Governança

> Status: proposta em piloto. Os times e a matriz de revisão abaixo partem dos times já criados na organização e devem ser confirmados pelos responsáveis.

## Times

| Time | Escopo |
|---|---|
| `team-ti` | Governança, infraestrutura, CI/CD, segurança e padrões da organização |
| `team-dados` | Desenvolvimento, integrações e inteligência de dados |
| `team-ecommerce` | Sistemas e integrações de e-commerce |
| `team-teste` | Validação de fluxos e pilotos de governança |

## Papéis

| Papel | Responsabilidade |
|---|---|
| Arquiteto | Decisões técnicas, ADRs, aprovação de spec e plano nas demandas |
| Revisor | Revisão de código; obrigatório em mudanças de autenticação, tokens e dados pessoais |
| Dono do repositório | Prioriza issues, aprova deleções e decide ações de achados de auditoria |
| Cético | Revisão independente, em contexto novo, que tenta refutar cada achado e conclusão; um achado só segue se sobreviver a um teste executado |

## Branches

| Branch | Uso | Regra |
|---|---|---|
| `main` | Fonte da verdade e produção | Só por pull request, com 1 aprovação; sem force push |
| `feature/*`, `fix/*`, `refactor/*`, `test/*`, `docs/*`, `chore/*`, `ci/*` | Trabalho | Criadas a partir da `main` |
| Ambientes (ex.: `hml`) | Validação | Recebem mudanças para teste; nunca são promovidos para a `main` |

## Revisão

1. Toda mudança na `main` entra por pull request.
2. No mínimo 1 aprovação; o autor não aprova a própria PR.
3. CI verde quando o repositório tiver CI.
4. Conversas resolvidas antes do merge.

| Área | Revisor obrigatório |
|---|---|
| CI/CD, infraestrutura, segurança e padrões | `team-ti` |
| Integrações, dados e ERP | `team-dados` |
| E-commerce e canais de venda | `team-ecommerce` |

## Decisões e documentação

- Decisão difícil de reverter, surpreendente sem contexto e com trade-off real vira ADR em `docs/adr/`.
- Procedimento operacional vira runbook em `docs/runbooks/`.
- Termos do domínio ficam no `GLOSSARY.md`.
- Documentos de processo (planos, evidências, handoffs) ficam fora do Git.
- Achados de auditoria e o acompanhamento do programa ficam no repositório privado de governança.

## Uso de IA

- Agentes seguem as mesmas regras de contribuição, revisão e prova.
- Código gerado por IA passa pelo mesmo processo de revisão e precisa de testes.
- Nenhum agente recebe ou registra segredo em texto.
