# winmoi-template

Template repository for your personal (can be private) [WinMoi](https://github.com/davinci42/WinMoi) Windows environment configuration.

## Layout

```text
manifest.toml            # Declarative Scoop buckets, packages, env, links, and skills
configs/<pkg>/           # Per-package config dirs linked bidirectionally via config_to
agent/skills/<skill>/    # Local private skills linked individually to ~/.agents/skills/<name>
```

## Usage

1. Create your own private repository from this template and clone it.
2. Edit `manifest.toml` (set `scoop.root`, packages, `config_to`, and skills).
3. Run:

```powershell
winmoi apply --dry-run
winmoi apply
winmoi status
```
