# win-tools

<!-- Project Shields/Badges -->
<p align="center">
  <a href="https://github.com/XAOSTECH/win-tools">
    <img alt="GitHub repo" src="https://img.shields.io/badge/GitHub-XAOSTECH%2F-win-tools-181717?style=for-the-badge&logo=github">
  </a>
  <a href="https://github.com/XAOSTECH/win-tools/releases">
    <img alt="GitHub release" src="https://img.shields.io/github/v/release/XAOSTECH/win-tools?style=for-the-badge&logo=semantic-release&colour=blue">
  </a>
  <a href="https://github.com/XAOSTECH/win-tools/blob/main/LICENCE">
    <img alt="Licence" src="https://img.shields.io/github/licence/XAOSTECH/win-tools?style=for-the-badge&colour=green">
  </a>
</p>

<p align="center">
  <a href="https://github.com/XAOSTECH/win-tools/actions">
    <img alt="CI Status" src="https://github.com/XAOSTECH/win-tools/actions/workflows/bash-lint.yml/badge.svg?branch=Main>
  </a>
  <a href="https://github.com/XAOSTECH/win-tools/issues">
    <img alt="Issues" src="https://img.shields.io/github/issues/XAOSTECH/win-tools?style=flat-square&logo=github&colour=yellow">
  </a>
  <a href="https://github.com/XAOSTECH/win-tools/pulls">
    <img alt="Pull Requests" src="https://img.shields.io/github/issues-pr/XAOSTECH/win-tools?style=flat-square&logo=github&colour=purple">
  </a>
  <a href="https://github.com/XAOSTECH/win-tools/stargazers">
    <img alt="Stars" src="https://img.shields.io/github/stars/XAOSTECH/win-tools?style=flat-square&logo=github&colour=gold">
  </a>
  <a href="https://github.com/XAOSTECH/win-tools/network/members">
    <img alt="Forks" src="https://img.shields.io/github/forks/XAOSTECH/win-tools?style=flat-square&logo=github">
  </a>
</p>

<p align="center">
  <img alt="Last Commit" src="https://img.shields.io/github/last-commit/XAOSTECH/win-tools?style=flat-square&logo=git&colour=blue">
  <img alt="Repo Size" src="https://img.shields.io/github/repo-size/XAOSTECH/win-tools?style=flat-square&logo=files&colour=teal">
  <img alt="Code Size" src="https://img.shields.io/github/languages/code-size/XAOSTECH/win-tools?style=flat-square&logo=files&colour=orange">
  <img alt="Contributors" src="https://img.shields.io/github/contributors/XAOSTECH/win-tools?style=flat-square&logo=github&colour=green">
</p>

<!-- Optional: Stability/Maturity Badge -->
<p align="center">
  <img alt="Stability" src="https://img.shields.io/badge/stability-experimental-orange?style=flat-square">
  <img alt="Maintenance" src="https://img.shields.io/maintenance/yes/2026?style=flat-square">
</p>

---

<p align="center">
  <b>Quality-of-life wrappers and utilities for Windows gaming and productivity</b>
</p>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Tools](#-tools)
- [Installation](#-installation)
- [Usage](#-usage)
- [Contributing](#-contributing)
- [Roadmap](#-roadmap)
- [Support](#-support)
- [Licence](#-licence)

---

## 🔍 Overview

A collection of FOSS wrappers and utilities for Windows. These tools focus on quality-of-life improvements for software that lacks certain features — without modifying, reverse-engineering, or patching the original applications.

### Why win-tools?

Some popular Windows applications — particularly game store launchers — are missing basic quality-of-life features that users have been requesting for years. Rather than wait, win-tools provides external wrappers that automate the tedious manual workarounds users already perform, using only public Windows APIs (registry reads, filesystem operations, process monitoring).

---

## 🧰 Tools

| Tool | Description | Status |
|------|-------------|--------|
| [**EGS-LL**](EGS-LL/) | Experienced Games Store Launcher Launcher — automates install recovery/verification | ✅ Active |

---

## 📥 Installation

### Prerequisites

- **Windows 10/11** with PowerShell 5.1+ (ships with Windows)
- The target application installed (e.g. Epic Games Store for EGS-LL)

### Quick Start

```powershell
# Clone the repository
git clone https://github.com/XAOSTECH/win-tools.git
cd win-tools

# Navigate to the desired tool
cd EGS-LL

# If needed, allow script execution for the current session
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser

# Run the tool
.\egs-ll.ps1 help
```

---

## 🚀 Usage

Each tool has its own README with detailed usage instructions. See the [Tools](#-tools) table above for links.

<details>
<summary>📘 Example: EGS-LL — Recover a game install</summary>

```powershell
# List all EGS-managed games
.\egs-ll.ps1 list

# Recover an existing game folder (automates the verify workaround)
.\egs-ll.ps1 recover "Red Dead Redemption 2"
```

</details>

---

## 🤝 Contributing

Contributions are welcome! Please read our [Contributing Guidelines](CONTRIBUTING.md) before submitting PRs.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

See also: [Code of Conduct](CODE_OF_CONDUCT.md) | [Security Policy](SECURITY.md)

---

## 🗺️ Roadmap

- [x] EGS-LL — Install recovery automation
- [x] EGS-LL — Game listing and EGS info display
- [ ] EGS-LL — Automated pause/resume via process monitoring
- [ ] Additional launcher wrappers (Steam, GOG, etc.)
- [ ] Unified CLI for all tools

See the [open issues](https://github.com/XAOSTECH/win-tools/issues) for a full list of proposed features and known issues.

---

## 💬 Support

- 💻 **Issues**: [GitHub Issues](https://github.com/XAOSTECH/win-tools/issues)
- 💬 **Discussions**: [GitHub Discussions](https://github.com/XAOSTECH/win-tools/discussions)

---

## 📄 Licence

Distributed under the GPL-3.0 Licence. See [`LICENCE`](LICENCE) for more information.

---

<p align="center">
  <a href="https://github.com/XAOSTECH">
    <img src="https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20by-XAOSTECH-red?style=for-the-badge">
  </a>
</p>

<p align="center">
  <a href="#win-tools">⬆️ Back to Top</a>
</p>
