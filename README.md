# .github

Arquivos de comunidade padrão da organização. O GitHub aplica cada arquivo daqui a todo repositório da organização que não tenha a sua própria versão.

| Arquivo | Efeito |
|---|---|
| `.github/PULL_REQUEST_TEMPLATE.md` | Template padrão de pull request |
| `.github/ISSUE_TEMPLATE/bug_report.yml` | Formulário "Bug" |
| `.github/ISSUE_TEMPLATE/feature_request.yml` | Formulário "Funcionalidade" |
| `.github/ISSUE_TEMPLATE/demanda.yml` | Formulário "Demanda com spec" |
| `.github/ISSUE_TEMPLATE/test_list.yml` | Formulário "Mudança com lista de testes" |
| `.github/ISSUE_TEMPLATE/infra.yml` | Formulário "Tarefa de infraestrutura" |
| `.github/ISSUE_TEMPLATE/postmortem.yml` | Formulário "Postmortem" |
| `.github/ISSUE_TEMPLATE/achado_auditoria.yml` | Formulário "Achado de auditoria" |
| `.github/ISSUE_TEMPLATE/config.yml` | Mantém issues em branco permitidas durante o piloto |
| `CONTRIBUTING.md` | Guia de contribuição padrão |
| `CODE_OF_CONDUCT.md` | Código de conduta |
| `GOVERNANCE.md` | Times, papéis, branches e revisão |
| `SECURITY.md` | Política de segurança padrão |

Um repositório que tenha a sua própria pasta `.github/ISSUE_TEMPLATE/` não herda nenhum formulário daqui; nesse caso, copie os que fizerem sentido.

Este repositório é público por exigência do GitHub para que os padrões sejam herdados. Não guarde aqui nada interno: segredos, nomes de sistemas, dados ou riscos ficam no repositório privado de governança.

Alterações entram por pull request.
