# NasTech-Agent Update Summary

> Powered by NousResearch

This verified NasTech-Agent update incorporates the newest confirmed improvements from its open-source foundation. The summary below focuses on delivered functionality, reliability, and operational impact.

## Update scope

- **Changes incorporated:** 254 commits affecting 2902 files.
- **Source revision:** `6a2662a4aaad`.
- **Previous source revision:** `73162b00eefd`.

## Technical coverage

- **.github/:** 7 changed files.
- **Dockerfile/:** 1 changed files.
- **acp_adapter/:** 3 changed files.
- **agent/:** 183 changed files.
- **apps/:** 92 changed files.
- **batch_runner.py/:** 1 changed files.
- **cli.py/:** 2 changed files.
- **contributors/:** 17 changed files.
- **cron/:** 14 changed files.
- **evals/:** 42 changed files.
- **gateway/:** 115 changed files.
- **justfile/:** 1 changed files.
- **lefthook.yml/:** 4 changed files.
- **locales/:** 3 changed files.
- **mcp_serve.py/:** 1 changed files.
- **nastech_bootstrap.py/:** 1 changed files.
- **nastech_cli/:** 299 changed files.
- **nastech_constants.py/:** 2 changed files.
- **nastech_logging.py/:** 1 changed files.
- **nastech_platform/:** 3 changed files.
- **nastech_startup_watchdog.py/:** 2 changed files.
- **nastech_state.py/:** 2 changed files.
- **nastech_state_common.py/:** 1 changed files.
- **nastech_state_dbfile.py/:** 1 changed files.
- **nastech_state_errors.py/:** 1 changed files.
- **nastech_state_guard.py/:** 1 changed files.
- **nastech_state_maintenance.py/:** 2 changed files.
- **nastech_state_portability.py/:** 1 changed files.
- **nastech_state_readpool.py/:** 2 changed files.
- **nastech_state_registry.py/:** 1 changed files.
- **nastech_state_repair.py/:** 1 changed files.
- **nastech_state_schema.py/:** 1 changed files.
- **nastech_state_search.py/:** 1 changed files.
- **nastech_state_sessions.py/:** 1 changed files.
- **nastech_yaml.py/:** 1 changed files.
- **optional-skills/:** 22 changed files.
- **package-lock.json/:** 2 changed files.
- **package.json/:** 3 changed files.
- **plugin-catalog/:** 82 changed files.
- **plugins/:** 96 changed files.
- **pm/:** 24 changed files.
- **providers/:** 1 changed files.
- **pyproject.toml/:** 1 changed files.
- **registration_lifecycle.py/:** 1 changed files.
- **ruff.pre-commit.toml/:** 2 changed files.
- **ruff.strict.toml/:** 9 changed files.
- **ruff.toml/:** 4 changed files.
- **run_agent.py/:** 2 changed files.
- **scripts/:** 56 changed files.
- **skills/:** 21 changed files.
- **tests/:** 920 changed files.
- **tools/:** 146 changed files.
- **trajectory_compressor.py/:** 4 changed files.
- **tui_gateway/:** 24 changed files.
- **utils.py/:** 2 changed files.
- **uv.lock/:** 2 changed files.
- **website/:** 59 changed files.

## Delivered improvements

### New capabilities

- feat(plugins): core-made Codex requests so plugins never hold the token
- feat(relay): emit compaction marks from the compression attempt record
- feat(plugin-catalog): add jp-edinet
- feat(plugin-catalog): add nastech-adaptive-effort plugin
- feat(plugin-catalog): add beam plugin
- feat(plugin-catalog): repin radio-dm-gateway to f3f8049 after the repository rename
- feat(plugin-catalog): remove old meshtastic-gateway file name
- feat(plugin-catalog): rename meshtastic-gateway to radio-dm-gateway
- feat(plugin-catalog): add meshtastic-gateway
- feat(plugin-catalog): bump command-ledger to 1.1.0
- feat(plugin-catalog): bump approval-ledger to 1.1.0
- feat(plugin-catalog): memory-shield 1.1.2 (review fixes)
- 13 additional new capabilities updates are included in this verified snapshot.

### Reliability and fixes

- fix: add tsx to linted extensions
- fix(checkpoints): avoid history queries in the footprint notice
- fix(install): name the marker owner as the Desktop hand-off pid
- fix(update): stable lookup failures travel as exceptions and name the quota the failed request spent
- fix(update): the stable lookup sends the user's GitHub token and names a rate limit as one
- fix(compression): a refused candidate's attempt record claims no effect
- fix(compression): keep a running attempt's record when an overlapping call stops at a gate
- fix(scripts): count only committed attempts as batch compactions in the micro-compaction report
- fix(relay): mark an in-place engine's archived compaction as a compaction
- fix(compression): name the guard that blocked an overflow attempt
- fix(shared-metrics): count an empty-transcript refusal under its own class
- fix(shared-metrics): limit bench alias to committed rows
- 72 additional reliability and fixes updates are included in this verified snapshot.

### Documentation

- docs(plugin-catalog): rule 11 — credentials come through Nastech, never from files
- docs(relay): document the summarizer fields as free-form identifiers
- docs(relay): list the gateway reset after compression exhaustion as unmarked
- docs(update): CLI reference names stable as the default and --set-channel main as the way back
- docs(skills): note inline-shell scoping for nested, external_dirs and unreadable-lock cases
- docs(telemetry): v4 takes additive values in place after its stable release
- docs(image_gen): state the fallback rule as no server accepted the request
- docs(tool-gateway): attribute the 429 retries to the gateway
- docs(loops): soften backend-lifetime wording

### Improvements

- Merge pull request #135838 from Nastechresearch/ci-speed-pt2
- ci: don't enforce CC in pre commit
- chore: pin specific js dependency versions
- ci: add js linting to pre commit hook
- ci: checkout once for docker and shell linting
- Merge pull request #135743 from Nastechresearch/harder-linter-fixes-part3
- fmt(js): `npm run fix` on merge (#136310)
- test(desktop): the source hand-off fixture installs its loopback transport once
- test(e2e): the Desktop update harness keeps the seed's channel record
- test(e2e): update sandboxes follow the main channel, not the stable default
- refactor(checkpoints): reuse _store_has_head in the footprint notice
- test: a relaunched hand-off update adopting its own claim runs on the macOS lane
- 124 additional improvements updates are included in this verified snapshot.

## Verification evidence

- **Direct source provenance:** Passed
- **Brand and asset integrity:** Passed
- **Dependency, security, and publication-readiness scans:** Passed
- **Full verification and fork-consistency checks:** Passed

This candidate is prepared for review only. No merge, release, or deployment is performed by the verification workflow.
