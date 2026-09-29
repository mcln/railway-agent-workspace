# railway-agent-workspace

**Status: work in progress. Nothing is built yet.** This repository currently contains only a licence and this README. It is not deployable, and there is no Railway template published from it.

## Intent

An unofficial, open-source workspace for running coding agents in the browser on [Railway](https://railway.com): a single service running [code-server](https://github.com/coder/code-server) (VS Code in the browser, with an integrated terminal) and one persistent volume for the home directory.

Planned design points, none of which are implemented or tested yet:

- Password authentication enforced at startup; the container refuses to start without a sufficiently long password
- Runs as a non-root user, no sudo, no SSH daemon, no TCP proxy
- code-server's port proxying and telemetry disabled
- tmux for long-running sessions
- Agent CLIs installed by the user on demand onto the volume, not bundled in the image

Before any public template is published, the Railway Acceptable Use Policy and Fair Use terms need to be read and checked against this design.

This project is not affiliated with or endorsed by Railway, Coder, or any agent vendor.

## Licence

MIT, see [LICENSE](LICENSE).
