# manman — Manager Master (最上位ダッシュボード)

`portmanager` / `portmap` / `nodeman` / `serverman` を束ねる統合 CLI。

## Commands

| Command | Description |
|---------|-------------|
| `manman ls` | Unified dashboard (ports + PIDs + skills) |
| `manman ps` | Show all processes (node + python + web servers) |
| `manman ports` | Port occupancy status |
| `manman servers` | Registered skill server status |
| `manman start <skill>` | Start skill server |
| `manman stop <skill\|port\|pid>` | Stop by skill/port/PID |
| `manman restart <skill>` | Restart skill |
| `manman open <skill>` | Open in browser |
| `manman health` | Health check all skills |
| `manman clean` | Remove migrated source dirs (1028, hokusai-manga) |
| `manman gc` | Cleanup temp files / npm cache |
| `manman win-check` | Check remaining dirs under C:\Users\0501JP\ |
| `manman register <name> <port> <dir> <cmd> [url]` | Register new skill |

## Install

```bash
chmod +x manman
ln -sf $(pwd)/manman ~/bin/manman
```

## Depends on

- `portmanager/` suite (portmanager, portmap, nodeman, serverman)
- bash
- powershell.exe (for Windows process/port queries)
