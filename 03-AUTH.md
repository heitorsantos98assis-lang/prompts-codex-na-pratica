# Prompt 03 — AUTH
## Login, sessão e controle de acesso com JWT

**Quando usar:** Para implementar autenticação em qualquer sistema.

---

## Prompt (copie e cole no Claude Code)

```
Preciso implementar autenticação completa no sistema [NOME DO SISTEMA].

Como o login vai funcionar:
- O usuário acessa via [email e senha / apenas email (magic link) / CPF e senha]
- Após login, ele deve ter acesso a [descreva as áreas protegidas]
- Níveis de acesso necessários: [ex: admin, gestor, usuário comum / apenas um nível]

Nossa stack:
- Backend: Node.js com Express no Coolify
- Frontend: Next.js com App Router na Vercel
- Auth: JWT armazenado em cookie httpOnly (NUNCA localStorage)
- Banco: PostgreSQL com pacote `pg`
- IMPORTANTE: não use Supabase Auth, NextAuth, Clerk ou qualquer biblioteca de auth externa

Com base nisso, implemente:
1. Rota POST /auth/login no backend que valida email+senha e retorna JWT
2. Rota POST /auth/logout que limpa o cookie
3. Rota GET /auth/me que retorna o usuário logado a partir do token
4. Middleware de autenticação para proteger rotas no backend
5. Middleware no Next.js (middleware.ts) que redireciona para /login se não autenticado
6. Hook useAuth() no frontend para acessar o usuário logado em qualquer componente
7. Página de login em /login com formulário funcional usando Origin UI
8. A senha deve ser armazenada com hash bcrypt — nunca em texto puro
```

---

## Dicas

- Cookie httpOnly é mais seguro que localStorage — o JavaScript não consegue ler
- Guarde o JWT_SECRET no `.env` com uma string longa e aleatória
- Se precisar de reset de senha no futuro, use este prompt acrescentando essa função
