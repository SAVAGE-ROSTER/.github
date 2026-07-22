# Contributing — the house law

Every talent site in this org is a face of the SAVAGE house and follows the
same law; a repo's own `CLAUDE.md`/README refines it, never relaxes it.

## The gates

Nothing ships red. Before any push:

```
pnpm typecheck && pnpm lint && pnpm build
```

All three green, every time. If a gate fails, fixing it comes before
anything else — broken steps never stack.

## The way

- **pnpm only.** No npm, no yarn.
- **TypeScript strict.** No `any` escape hatches, no `@ts-ignore` drive-bys.
- **Branch → PR → merge.** No direct pushes to `main`.
- **The brand is locked.** Every face carries the house aesthetic — dark
  luxe, brand tokens only, gold as foil, marks never redrawn. Per-talent
  accents live inside the token system, never beside it.
- **Faces stay thin.** Talent sites read and render; every write POSTs to
  the MACHINE's public contract. No local backends, no face-side auth.
- **New talent starts from TALENT-TEMPLATE.** The stamp, not a fork of a
  sister site.
- **No secrets on disk or in code.** Credentials live in the vault; env
  resolves at run time.

## Commits

Conventional commits (`feat:`, `fix:`, `docs:`, `chore:`), scoped and
specific. Say what shipped, not what you did.
