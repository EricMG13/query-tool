# Query Tool

Work and documentation for the Query Tool: a local, conversational assistant that answers questions about issuers using the analysis our credit workflow has already produced.

| Folder | Contents |
|---|---|
| [presentation/](presentation/) | Slide content for presenting the application and the Query Tool to a non-technical audience |

## Related material elsewhere

- Design, plan and test evidence: `~/Documents/features list/Query Tool/` (start with its README and the implementation plan in `docs/superpowers/plans/`).
- Working prototype: `~/Documents/issuer-knowledge-app/`, branch `feature/local-knowledge`.
- The analytical workflow and the Issuer Library application: `~/Documents/final-workflow/`.

## Current decisions

- Storage: PostgreSQL running on the user's own computer (decided 2026-11-10). The prototype still uses SQLite.
- Knowledge is held as readable Markdown notes in an OKF-based format; the database is an index that can be rebuilt from them.
- Only analysis that someone explicitly adds to the library can be used in answers.
- Status: prototype tested on one historical case. AI-written answers, search by meaning and web research are not built yet.
