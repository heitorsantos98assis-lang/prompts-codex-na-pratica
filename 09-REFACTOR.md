# Prompt 09 — REFACTOR
## Reorganizar código bagunçado sem quebrar nada

**Quando usar:** Quando o projeto cresceu e está difícil de entender ou manter.

---

## Prompt (copie e cole no Claude Code)

```
O código do sistema [NOME DO SISTEMA] cresceu e está ficando difícil de manter.

O problema que estou sentindo:
[ex: o arquivo routes.js virou um monstro com 800 linhas e não acho mais nada]
[ex: toda vez que mudo uma coisa, quebra outra em lugar diferente]
[ex: tem código repetido em vários lugares e fica inconsistente]

Área do código com problema:
[ex: o backend todo / apenas as rotas de leads / os componentes do dashboard]

Nossa stack:
- Backend: Node.js com Express no Coolify
- Frontend: Next.js com App Router na Vercel
- Banco: PostgreSQL com `pg`

Por favor:
1. Analise os arquivos da área descrita e mostre o que está errado
2. Proponha uma estrutura melhor antes de mudar qualquer coisa
3. Faça a reorganização de forma gradual, um arquivo por vez
4. Confirme que nada quebrou depois de cada mudança
5. Me mostre a diferença entre como estava e como ficou
```

---

## Dicas

- Peça para o Claude analisar ANTES de mudar — assim você aprova o plano primeiro
- Faça refactor em partes pequenas, não tudo de uma vez
- Sempre rode o sistema depois do refactor para confirmar que continua funcionando
