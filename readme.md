# ⚫ @collide-kit/collide-rnvt

[![CI](https://github.com/collide-kit/collide-rnvt/actions/workflows/ci.yml/badge.svg)](https://github.com/collide-kit/collide-rnvt/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

🤖 Collide Tech default [Renovate](https://docs.renovatebot.com/) preset

## 📦 Usage

Add to your `renovate.json` (or `renovate.json5`, `.renovaterc`):

```json
{
  "extends": ["github>collide-kit/collide-rnvt"]
}
```

---

## ⚙️ What's included

| Setting                                      | Value                      | Description                                               |
| -------------------------------------------- | -------------------------- | --------------------------------------------------------- |
| Base                                         | `config:recommended`       | Renovate recommended defaults                             |
| Schedule                                     | `weekly`                   | PRs created once a week                                   |
| Grouping                                     | `group:allNonMajor`        | All minor/patch updates grouped into one PR               |
| `minimumReleaseAge`                          | `3 days`                   | Skips packages published less than 3 days ago             |
| `rangeStrategy`                              | `bump`                     | Bumps version inside the range (e.g. `^1.2.0` → `^1.3.0`) |
| `automergeStrategy`                          | `squash`                   | Squash-merges automerged PRs                              |
| `platformAutomerge`                          | `true`                     | Uses platform-native automerge                            |
| `semanticCommits`                            | `disabled`                 | Disables semantic commit detection                        |
| `commitMessagePrefix`                        | `🧩 chore(deps):`          | Prefix for all dependency commit messages                 |
| `commitMessageAction`                        | `update`                   | Commit message action verb                                |
| `labels`                                     | `dependencies`             | Applied to all dependency PRs                             |
| `timezone`                                   | `Europe/Zurich`            | Schedule runs in CET/CEST                                 |
| `dependencyDashboardTitle`                   | `🔄 Dependency Dashboard`  | Custom dashboard issue title                              |
| `dependencyDashboardAutoclose`               | `true`                     | Closes dashboard issue when no open PRs remain            |
| `dependencyDashboardOSVVulnerabilitySummary` | `unresolved`               | Shows only unresolved OSV vulnerabilities                 |
| `vulnerabilityAlerts.enabled`                | `true`                     | Enables Renovate vulnerability PRs                        |
| `vulnerabilityAlerts.labels`                 | `dependencies`, `security` | Labels applied to vulnerability PRs                       |

---

## 📦 Package rules

- ❌ **`peerDependencies`** — disabled (not managed by Renovate)
- ✅ **`devDependencies` patch** — automerged when CI passes
- 🏷 **major updates** — labeled with `dependencies` and `major`
- 🔐 **security updates** — labeled with `dependencies` and `security`

---

## 📄 License

MIT © 2026 CollideKit

---

**Made with ⚫ by [gratisv](https://github.com/gratisv)**
