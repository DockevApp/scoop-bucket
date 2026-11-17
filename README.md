<h1 align="center">Dockev for Windows</h1>

<p align="center">
  Official <a href="https://scoop.sh">Scoop</a> bucket for <a href="https://github.com/DockevApp/Dockev"><b>Dockev</b></a>, the desktop app for Docker.
</p>

<p align="center">
  <img alt="Latest version" src="https://img.shields.io/badge/version-0.7.0-2563eb">
  <img alt="Architecture" src="https://img.shields.io/badge/arch-x64-475569">
  <img alt="scoop" src="https://img.shields.io/badge/scoop-bucket-16a34a">
</p>

<p align="center">
  <a href="#install">Install</a> ·
  <a href="#update">Update</a> ·
  <a href="#uninstall">Uninstall</a> ·
  <a href="#other-platforms">Other platforms</a>
</p>

---

## Install

Windows 10 / 11 (x64). No admin rights needed.

**1. Add the bucket**

```powershell
scoop bucket add dockev https://github.com/DockevApp/scoop-bucket
```

**2. Install**

```powershell
scoop install dockev
```

Open **Dockev** from the Start menu.

<details>
<summary><b>Don't have Scoop yet?</b></summary>

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

See [scoop.sh](https://scoop.sh) for details.

</details>

---

## Update

```powershell
scoop update dockev
```

Scoop installs update through Scoop, not from inside the app. Dockev detects this and shows the command above when a new version is out.

---

## Uninstall

```powershell
scoop uninstall dockev
scoop bucket rm dockev
```

<details>
<summary><b>Remove settings and data too</b></summary>

```powershell
Remove-Item -Recurse -Force "$env:APPDATA\com.nacasha.dockev", "$env:LOCALAPPDATA\com.nacasha.dockev" -ErrorAction SilentlyContinue
```

</details>

---

## Other platforms

| Platform | Install |
|---|---|
| **macOS** | `brew install --cask dockevapp/dockev/dockev` |
| **Linux** (apt, dnf, zypper, pacman) | [dockevapp.github.io/packages](https://dockevapp.github.io/packages) |
| **Windows installer** (.msi / .exe) | [Download from GitHub Releases](https://github.com/DockevApp/Dockev/releases/latest) |
