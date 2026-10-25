# ContextQA learning lab: HTML and vanilla JavaScript TodoMVC

This is a public educational fork of [tastejs/todomvc](https://github.com/tastejs/todomvc). Original source, history, licenses and attribution are retained. It is not a customer production application.

## Status

Source is available. Hosted full-stack sessions and ContextQA reports are not yet verified for this track. The exercises below are a test-design guide, not a passing test report. Upstream starting commit: `ff43b02e59dfa604386bb382034b2cd07c2bcd8a`.

## Run locally

Start with examples/javascript-es5/dist/index.html through an HTTP static server. The upstream repository includes multiple frameworks; this lab focuses on its vanilla JavaScript implementation. State lives in browser localStorage, so use a clean browser profile per remote run. This is an introductory exercise, not an enterprise benchmark.

See the [upstream setup guide](../README.md#upstream-project-documentation) for the project's original instructions.

## Exercises

| Scenario | Required assertion |
|---|---|
| Add | Two uniquely named tasks appear after Enter. |
| Edit | Double-clicking and saving changes a task title. |
| Complete and filter | A completed task appears under Completed and is absent under Active. |
| Persistence | A task and its completion status remain after reload. |
| Clear completed | Clearing completed tasks removes only completed tasks. |

## Reproduce the end-to-end workflow

1. Start your own local or hosted copy with synthetic fixtures. ContextQA's cloud runner needs a reachable address; localhost needs a separately supported connection.
2. Choose one scenario and write explicit expected results before generating the test.
3. Follow [ContextQA's getting-started guide](https://contextqa.com/tutorials/getting-started-with-contextqa-test-automation/) or the [MCP documentation](https://mcp.contextqa.com/docs/faq) using your own authenticated workspace.
4. Create/review the test steps, execute, and inspect the actual assertion and runner verdict.
5. Introduce one disclosed regression in a separate local branch. Repeat the same test, observe failure, fix the application and rerun.
6. Record the app commit, fixture/scenario version, browser, tool version, timestamp, step counts and evidence. Do not describe a recording as a fresh run.
7. Repeat on a URL you own or have permission to test. Use synthetic data and confirm actions that submit or alter records.

## Reports and limitations

No ContextQA report is included yet. Add only actual execution evidence. Public reports must contain synthetic data and explicit provenance. Private target results must stay private. Upstream tests remain upstream tests; they are not proof of a ContextQA run.

Recorded reports can be reused for the exact pinned fixture and version. Live runs need fresh isolated state and quotas. Code export, CI integration, automatic resets and embedded execution should be demonstrated only after independently verified.

## Teaching brief

Show the app, source and assertion; create and run the test; inspect evidence; reproduce a regression; show the fix; then test an authorized app of your own. Keep setup and execution time separate. Link the exact release and acknowledge upstream creators. Creator sponsorships should be disclosed.
