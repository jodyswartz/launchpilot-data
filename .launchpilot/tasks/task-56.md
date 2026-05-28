# LaunchPilot Task #56

Repo: jodyswartz/launchpilot-data
Base branch: main
Branch: launchpilot/task-56-1779977580092

## Idea

Update the README for launchpilot-data. Explain that this repo stores the sanitized public dashboard export for LaunchPilot, especially tasks.json used by launchpilot-dashboard. Document that private repo tasks are filtered out by LaunchPilot before export using PUBLIC_DASHBOARD_REPOS, and that this repo should not contain secrets, private task prompts, private repo names, logs from private repos, or sensitive PR/deployment links. Add a short “How it fits” section explaining the three-repo setup: launchpilot generates the data, launchpilot-data stores tasks.json, and launchpilot-dashboard reads and displays it. Keep it concise and beginner-friendly.