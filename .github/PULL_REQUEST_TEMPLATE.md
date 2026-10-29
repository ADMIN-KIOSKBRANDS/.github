> [!CAUTION]
> **Barra lateral obrigatória antes de pedir revisão:** Assignees (quem implementou), Reviewers (ao menos 1, ver CODEOWNERS do repositório), Labels (tipo e prioridade), Milestone (onda ou sprint) e issue vinculada (`Closes #N` ou `Relates #N`).

## Descrição

- **Issue relacionada:** Closes #<!-- número -->
- **Contexto:** <!-- Por que esta mudança é necessária? -->

## Tipo de mudança

<!-- O prefixo do título segue Conventional Commits. -->

- [ ] `feat` — nova funcionalidade
- [ ] `fix` — correção de bug
- [ ] `refactor` — refatoração sem mudar comportamento
- [ ] `docs` — só documentação
- [ ] `test` — testes
- [ ] `perf` — desempenho
- [ ] `ci` / `chore` — CI, dependências, configuração
- [ ] Quebra compatibilidade (`feat!` ou `fix!`)

## Rastreabilidade

| Item | Referência |
|------|-----------|
| Spec ou demanda | <!-- issue, link ou N/A --> |
| ADR relacionado | <!-- docs/adr/NNNN-... ou N/A --> |
| Runbook afetado | <!-- docs/runbooks/... ou N/A --> |
| Regras de negócio (IDs) | <!-- ex.: NFE-06, ou "Nenhuma" --> |

## Causa raiz

<!-- Obrigatório em fix: por que a falha acontecia, com `arquivo:linha`.
     Em feat: a lacuna que originou a mudança. -->

## Implementação

<!-- O que mudou: arquivos, funções, fluxos. Use `arquivo:linha`. -->

-

## Evidências

> [!WARNING]
> Sem evidência executada, sem merge. Cole o comando e a saída lida; nunca valores de segredo.

<details>
<summary>Antes — comportamento anterior</summary>

```
<!-- comando e saída -->
```

</details>

<details>
<summary>Depois — comportamento corrigido</summary>

```
<!-- mesmo comando, saída nova -->
```

</details>

| Tipo | Comando | Resultado |
|------|---------|-----------|
| Testes | <!-- ex.: npm test, pytest --> | <!-- N pass, 0 fail --> |
| Build ou lint | <!-- se houver --> | |
| Manual | <!-- cenário --> | |

- [ ] O teste novo falha sem a mudança e passa com ela.

## Impacto

- [ ] Não expõe segredo, token, senha nem dado pessoal (código, logs, commits).
- [ ] `.env`, bancos, dumps e logs continuam fora do Git.
- [ ] Não muda esquema de banco; se mudar, a migração está descrita acima.
- [ ] Não altera contrato de API consumido por outro sistema; se alterar, os consumidores estão listados.

## Checklist

- [ ] Título em Conventional Commits.
- [ ] Revisei o próprio diff.
- [ ] Documentação atualizada (README, ADR, runbook) quando aplicável.
- [ ] Documentos de processo (planos, handoffs, evidências) ficaram fora do Git.
- [ ] Esta PR contém código gerado por IA, com testes e suíte verde confirmada.
- [ ] Esta PR **não** contém código gerado por IA.
