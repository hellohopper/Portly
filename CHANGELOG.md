# Changelog

All notable changes to Portly are documented here. Format loosely follows
[Keep a Changelog](https://keepachangelog.com/).

## [0.2.0] - 2026-07-01

### Added
- Search/filter box in the dropdown — matches port, process name, framework label, project name, and git branch
- Pin favorites to the top of the list; remaining ports grouped alphabetically by project (with an "Other" bucket)
- Notifications when a new port starts listening, or when a pinned port stops unexpectedly
- Docker awareness — flags ports forwarded through Docker Desktop's host process with a badge, and makes them searchable via "docker"
- Bulk selection: select multiple rows and kill them in one action
- In-app update check against GitHub Releases, with a banner linking to the new version when available

## [0.1.0] - 2026-07-01

Initial release.

### Added
- Live list of listening TCP/UDP ports, refreshed every 2s, deduped across IPv4/IPv6 and merged into one row when a process listens on both protocols for the same port
- Git project context — repo name and current branch, resolved from the process's working directory (including worktree checkouts)
- Uptime, CPU%, and memory% per process, plus a color-coded energy indicator
- Framework-aware labeling (Vite, Next.js, Rails, Django, Flask, FastAPI, Node, Bun, Deno, and more)
- Kill a process, reveal its owning Terminal.app tab, open `localhost:<port>` in the browser, or copy the URL
- Global hotkey (Cmd+Shift+P) to toggle the menu
- System/Light/Dark theme toggle
- DMG installer, SHA-256 checksum publishing, and a Homebrew tap (`hellohopper/portly`)
- MIT license, showcase website ([hellohopper.github.io/portly](https://hellohopper.github.io/portly/))

[0.2.0]: https://github.com/hellohopper/portly/releases/tag/v0.2.0
[0.1.0]: https://github.com/hellohopper/portly/releases/tag/v0.1.0
