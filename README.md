# launchpilot-data

This repo stores the sanitized public dashboard export for LaunchPilot.
Its main file is `tasks.json`, which is read by `launchpilot-dashboard`.

## How it fits

- `launchpilot` generates the dashboard data.
- `launchpilot-data` stores the exported `tasks.json`.
- `launchpilot-dashboard` reads `tasks.json` and displays it.

Before export, LaunchPilot filters out private repo tasks using
`PUBLIC_DASHBOARD_REPOS`. This repo should only contain data that is safe to
show publicly.

Do not commit secrets, private task prompts, private repo names, logs from
private repos, or sensitive PR/deployment links.
