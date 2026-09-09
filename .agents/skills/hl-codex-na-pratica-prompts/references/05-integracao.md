# Prompt 05 — INTEGRAÇÃO
## Conectar APIs externas: WhatsApp, Stripe, Meta Ads e outras

**Quando usar:** Para conectar o sistema a qualquer serviço externo.

---

## Prompt para o Codex

```
Preciso integrar o sistema com [NOME DA API/SERVIÇO].

O que a integração precisa fazer:
- [ex: enviar mensagem de WhatsApp quando um lead for cadastrado]
- [ex: processar pagamento quando o usuário clicar em comprar]
- [ex: buscar métricas de campanhas do Meta Ads diariamente]
- [descreva o fluxo completo]

Detalhes da integração:
- API: [ex: WhatsApp Business API Oficial / Stripe / Meta Ads API]
- Quando dispara: [ex: ao salvar um formulário / automaticamente todo dia às 8h / quando o usuário clicar no botão]
- O que fazer com o retorno: [ex: salvar no banco / mostrar na tela / enviar email]

Nossa stack:
- Backend: Node.js com Express no Coolify
- Frontend: Next.js na Vercel
- Banco: PostgreSQL com `pg`
- As credenciais da API ficam no .env do backend — NUNCA no frontend

Com base nisso:
1. Crie o serviço de integração no backend (arquivo separado em /services)
2. Crie a rota no Express que o frontend vai chamar
3. Trate os erros — se a API externa cair, o sistema não pode quebrar
4. Salve logs das chamadas no banco para rastrear problemas
5. Mostre como configurar as variáveis de ambiente necessárias
```

---

## Dicas

- Nunca coloque chaves de API no frontend — sempre passe pelo backend
- Peça ao Codex para criar um modo de teste antes de usar créditos reais da API
- Se a integração precisar de webhook (a API te chama), mencione isso no prompt
