# Cloudflare Pages + Workers + D1

Constraint: "Cloudflare first, other if not possible". Campus scale is tiny (hundreds of facilities, a few hundred daily users), so the free/cheap tier must suffice and no Postgres cluster is needed day one.

We decided: PWA frontend on Cloudflare Pages, API as a Worker, data in D1 (SQLite), email (verification codes) via Resend. Documented fallback: Workers + external Postgres via Hyperdrive if D1 limits are ever hit.
