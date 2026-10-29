# Política de segurança

Vale para todos os repositórios da organização que não tenham política própria.

## Como reportar

Não abra issue pública para vulnerabilidade. Avise o time de TI pelo canal interno ou use a opção **Report a vulnerability** da aba Security do repositório afetado.

Informe o repositório, o caminho do arquivo, como reproduzir e o impacto. Nunca cole o valor de um segredo: cite `caminho:linha`.

## Segredos e dados

- `.env`, chaves, tokens, certificados e bancos de dados não entram no Git. Use variáveis de ambiente no provedor de deploy.
- O `.gitignore` de todo repositório cobre `.env`, `*.env`, `*.db`, `*.sqlite`, `*.pem` e `*.key`.
- Segredo que chegou a um commit é tratado como exposto: rotacione antes de remover. Remover o arquivo não o tira do histórico.
- Reescrita de histórico só com aprovação do dono do repositório.
