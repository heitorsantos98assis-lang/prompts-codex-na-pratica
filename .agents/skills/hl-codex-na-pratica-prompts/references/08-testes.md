# Prompt 08 — TESTES
## Gerar testes automatizados sem escrever uma linha

**Quando usar:** Antes de fazer deploy ou depois de uma funcionalidade pronta.

---

## Prompt para o Codex

```
Preciso criar testes para o sistema [NOME DO SISTEMA / FUNCIONALIDADE].

O que quero testar:
- [ex: o fluxo de login — email correto entra, email errado é bloqueado]
- [ex: o cadastro de lead — campos obrigatórios, duplicidade de email]
- [ex: a rota de listagem — retorna os dados certos, não retorna dados de outros usuários]

Nossa stack:
- Backend: Node.js com Express
- Banco: PostgreSQL com `pg`
- Frontend: Next.js

Por favor:
1. Crie os testes para os cenários descritos acima
2. Use o framework mais simples possível para a nossa stack (não precisa ser complexo)
3. Configure o ambiente de teste para não usar o banco de produção
4. Mostre como rodar os testes com um único comando
5. Explique o que cada teste está verificando em linguagem simples
```

---

## Dicas

- Comece testando o que for mais crítico: login e as ações principais do sistema
- Um teste que passa não significa que está tudo certo — descreva cenários de falha também
- Se um teste quebrar depois de uma atualização, use o Prompt 06 (Debug) para investigar
