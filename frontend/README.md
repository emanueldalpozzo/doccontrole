# DocControle — Frontend

Este diretório vai concentrar a aplicação Next.js (React + TypeScript) que consome a API Laravel em [`/backend`](../backend). Ainda não foi feito o scaffold — este arquivo existe apenas para documentar o que está planejado, já que a Etapa 1 do projeto cobre apenas planejamento, não implementação.

## Stack planejada
- **Next.js** (App Router) + **React** + **TypeScript**
- **Tailwind CSS** para estilização
- Autenticação via **Laravel Sanctum** (SPA authentication, cookies same-site) contra a API em `/backend`

## Próximos passos (fora do escopo da Etapa 1)
1. Rodar `npx create-next-app@latest` dentro desta pasta com TypeScript, Tailwind e App Router.
2. Configurar cliente HTTP apontando para a API Laravel (`NEXT_PUBLIC_API_URL`).
3. Implementar fluxo de autenticação Sanctum (cookie CSRF + login).
4. Construir as telas mapeadas em `docs/wireframes` (a produzir em etapa futura).
