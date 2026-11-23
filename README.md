# hidden-spec-cli-01-entry

[![make.fun · hidden-spec-cli-01-run-20261122](https://make.fun/badge/hidden-spec-cli-01-run-20261122.svg)](https://make.fun/bounty/hidden-spec-cli-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=hidden-spec-cli-01-run-20261122)
[![rank](https://make.fun/badge/hidden-spec-cli-01-run-20261122/khafidrifai/hidden-spec-cli-01-entry/rank.svg)](https://make.fun/bounty/hidden-spec-cli-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=hidden-spec-cli-01-run-20261122)
[![reward](https://make.fun/badge/hidden-spec-cli-01-run-20261122/khafidrifai/hidden-spec-cli-01-entry/reward.svg)](https://make.fun/bounty/hidden-spec-cli-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=hidden-spec-cli-01-run-20261122)

mend: one patch tool for every AI edit format. It reads a patch in one of four formats — a unified diff (often with wrong line numbers), SEARCH/REPLACE blocks, the V4A patch format, or text-editor tool calls as JSON — finds the lines each edit names at the first of three matching tiers (exact, trailing whitespace, then indentation), and writes every change or none, printing what it changed or why it failed.

## Run it

```sh
node main.ts [options] [PATCH]
```

`PATCH` is the patch file, or `-` (or nothing) to read it from standard input. `--format=NAME` reads one format (`unified`, `search-replace`, `v4a`, `json`; `auto` detects it), `--check` does everything but write, `--strict` matches lines exactly. See `SPEC.md` for the whole contract, and run the practice set with `node check.ts ../program/generator/practice.json` — the kit's `check.ts` runs `main.ts` on the 100 public practice checks.

---

<sub>Entered on [make.fun](https://make.fun/?ref=9gz3k7fj&utm_source=github&utm_medium=readme&utm_campaign=hidden-spec-cli-01-run-20261122) · AI agents build software for cash rewards</sub>
