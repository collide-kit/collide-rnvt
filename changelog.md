# ⚫ @collide-kit/collide-rntv

## 1.0.0 🚀

### Major Release

🎉 **Initial release of `@collide-kit/collide-rntv`**

The first stable release of **@collide-kit/collide-rntv**

### ✨ Features

- **`default.json`** — shareable Renovate configuration preset
  - 📅 Weekly update schedule (`schedule:weekly`) in `Europe/Zurich` timezone
  - 📦 All non-major updates grouped into a single PR (`group:allNonMajor`)
  - 🛡️ 3-day minimum release age to avoid unstable packages
  - ⬆️ `rangeStrategy: bump` keeps dependency ranges in sync with installed versions
  - 🔀 `automergeStrategy: squash` for automerged PRs
  - 🔄 `platformAutomerge: true` enables platform-native automerge
  - 🚫 `semanticCommits: disabled`
  - 💬 Commit messages formatted as `🧩 chore(deps): update <package>`
    - `commitMessagePrefix: 🧩 chore(deps):`
    - `commitMessageAction: update`
  - 🏷️ `dependencies` label applied to all PRs
  - 🏷️ `major` label automatically added for breaking updates
  - 🔐 `peerDependencies` updates disabled
  - ✅ Automerge for `devDependencies` patch updates (when CI passes)
  - 📊 Dependency Dashboard
    - Title: `🔄 Dependency Dashboard`
    - Auto-closes when no open dependency PRs remain
    - Shows unresolved OSV vulnerabilities only
  - 🔐 Vulnerability alerts enabled
    - Security PRs labeled with `dependencies` and `security`
