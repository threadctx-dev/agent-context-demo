# agent-context-demo

A small repository whose AI agent instructions have drifted on purpose, to show
[threadctx](https://www.npmjs.com/package/threadctx) and its
[GitHub Action](https://github.com/threadctx-dev/action) at work.

- `AGENTS.md` says pnpm; `CLAUDE.md` says npm. The lockfile says pnpm.
- Claude Code never reads `AGENTS.md` here, because `CLAUDE.md` exists.

Open pull requests to see the grade-change comment. Try it yourself:

```bash
npx threadctx scan --github threadctx-dev/agent-context-demo
npx threadctx explain src/math.ts
```
