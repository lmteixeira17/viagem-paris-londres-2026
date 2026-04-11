# Instruções do projeto — viagem-paris-londres-2026

## Fluxo de publicação

Este é um site pessoal de itinerário de viagem (publicado via GitHub Pages a partir da branch `main`). O repositório é usado **durante a viagem** para consulta no celular, então mudanças precisam aparecer publicadas rápido.

### Regra de merge

**Sempre que houver uma implementação concluída, fazer merge direto na `main`** — sem abrir Pull Request.

Fluxo padrão após terminar uma alteração:

1. Commit na branch de trabalho designada
2. `git push -u origin <branch>`
3. `git checkout main && git pull origin main`
4. `git merge <branch> --no-ff -m "Merge: <descrição curta>"`
5. `git push -u origin main`
6. Voltar para a branch de trabalho se ainda for continuar: `git checkout <branch>`

Essa diretriz foi autorizada explicitamente pelo dono do repositório e substitui o comportamento padrão de "nunca fazer push em branch diferente da designada sem permissão" e "não criar PR sem pedido explícito" — aqui o merge direto é o comportamento esperado.

### Exceções

- Se a alteração for experimental/em dúvida, avisar antes de fazer merge.
- Se houver conflitos não-triviais com a `main`, parar e pedir orientação.
- Nunca usar `--force` ou `--no-verify`.
