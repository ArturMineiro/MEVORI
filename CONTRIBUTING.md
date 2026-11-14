# Como contribuir

## Tarefas
Todas as tarefas ficam no banco **Tarefas** do Notion. Cada uma tem um ID no formato `SAAS-n`.

## Fluxo
1. Pegue uma tarefa no quadro e mova para **Em andamento**.
2. Crie uma branch a partir da `main`:
   ```
   git checkout -b feature/SAAS-22-login-jwt
   ```
3. Faça commits no padrão [Conventional Commits](https://www.conventionalcommits.org/pt-br/) com o ID no fim:
   ```
   feat(auth): login com JWT [SAAS-22]
   fix(os): corrige cálculo de prazo [SAAS-31]
   ```
   Tipos: `feat`, `fix`, `chore`, `docs`, `refactor`, `test`, `style`.
4. Abra um Pull Request com o ID no título. O Notion vincula o PR à tarefa automaticamente.

## Configuração (uma vez por máquina)
Ative o hook que bloqueia commits sem ID:
```
git config core.hooksPath .githooks
```
