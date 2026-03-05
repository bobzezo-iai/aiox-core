# SM Agent Memory — River (Facilitator)

## Project: Ciclo das Estacoes

### Story Location
- Stories ativas: `docs/stories/active/`
- Numeracao: `E{epic}.{story}.story.md`
- Config `devStoryLocation: docs/stories` (nao `docs/stories/active`) — stories ficam em `active/`

### Story Template Padrao (sem story-tmpl.yaml disponivel)
Estrutura usada com sucesso neste projeto:
- Frontmatter YAML (id, title, status, epic, story, created, prd_ref, sprint)
- Story (Como / Quero / Para)
- Description (contexto + PRD reference)
- Acceptance Criteria (checkboxes `- [ ]`)
- Tasks / Subtasks (checkboxes `- [ ]`)
- Dev Notes (detalhes tecnicos + source references)
- CodeRabbit Integration (story type, complexity, agents, quality gates)
- File List (placeholder vazio)

### PRD do Projeto
- Path: `docs/prd/ciclo-das-estacoes-app.md`
- Stack: Next.js 15, Turborepo, pnpm, Prisma, Supabase, NextAuth v5, MercadoPago, Stripe, Resend, Vercel
- RBAC: 5 roles — VISITOR, USER, THERAPIST, FACILITATOR, ADMIN

### Agrupamentos de Stories Decididos
- E3.2 + E3.3 (PRD) → E3.2 "Payment Gateway" (MercadoPago + Stripe numa story)
- E3.4 (webhooks PRD) → E3.3
- E3.5 (QR Code) → E3.4
- E3.6 (cancelamento) → E3.5
- E3.7 (cross-selling) → E3.6
- Total: 24 stories (5+6+6+7) para 21 items do PRD

### template-tmpl.yaml
Nao existe em `.aiox-core/development/templates/story-tmpl.yaml` — apenas templates YAML de squads e workflows.
