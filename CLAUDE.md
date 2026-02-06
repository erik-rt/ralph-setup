## Plan Mode

- Make the plan extremely concise. Sacrifice grammar for the sake of concision.
- At the end of each plan, give me a list of unresolved questions to answer, if any.

## Tracer Bullets

When building features, build a tiny, end-to-end slice of the feature first, seek feedback, then expand out from there.

Tracer bullets comes from the Pragmatic Programmer. When building systems, you want to write code that gets you feedback as quickly as possible. Tracer bullets are small slices of functionality that go through all layers of the system, allowing you to test and validate your approach early. This helps in identifying potential issues and ensures that the overall architecture is sound before investing significant time in development.

## Feedback Loops

Before committing, run ALL feedback loops:

1. TypeScript: bun run check (must pass with no errors)
2. Tests: bun run test (must pass)
3. Lint: bun run lint (must pass)
4. e2e Tests: bun run test:e2e (must pass)
5. Visual Testing: Use the Playwright MCP server to verify no visual regressions.
   Do NOT commit if any feedback loop fails. Fix issues first.
