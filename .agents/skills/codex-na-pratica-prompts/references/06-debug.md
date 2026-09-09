# Prompt 06 — DEBUG
## Encontrar e corrigir erros sem entender o código

**Quando usar:** Sempre que algo quebrar ou não funcionar como esperado.

---

## Prompt para erro com mensagem

```
O sistema está com um erro e não consigo resolver.

O que eu fiz antes do erro aparecer:
[descreva o que você estava fazendo, ex: cliquei em salvar no formulário de leads]

A mensagem de erro que apareceu:
[cole aqui a mensagem de erro completa — pode ser do terminal, do browser ou da tela]

Onde o erro aparece:
[ex: no terminal do backend / no console do browser / na tela para o usuário]

Nossa stack:
- Frontend: Next.js (App Router) na Vercel
- Backend: Node.js com Express no Coolify
- Banco: PostgreSQL com `pg`

Por favor:
1. Explique em linguagem simples o que está causando o erro
2. Mostre exatamente o que precisa ser corrigido
3. Corrija o arquivo com problema
4. Me diga como confirmar que o erro foi resolvido
```

---

## Prompt — Comportamento errado sem mensagem de erro

```
O sistema não está se comportando como deveria, mas não aparece nenhum erro.

O que deveria acontecer:
[ex: ao clicar em salvar, o lead deveria aparecer na listagem]

O que está acontecendo de fato:
[ex: o formulário fecha, mas o lead não aparece na lista — só aparece se eu atualizar a página]

Por favor:
1. Identifique onde está o problema (frontend, backend ou banco)
2. Explique por que está acontecendo em linguagem simples
3. Corrija o problema
4. Confirme que o fluxo completo está funcionando depois da correção
```

---

## Dicas

- Cole o erro completo — nunca resuma a mensagem, ela tem informações importantes
- Se o erro aparecer no terminal do Coolify, vá em Logs no painel e copie tudo
- Se não souber onde ver o erro, diga ao Codex e ele vai te ensinar onde procurar
