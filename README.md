# Pitwall Mem

Local-first persistent memory for Claude Code: it records what happens in your sessions, compresses it with a local model through Ollama (never your Claude plan), and gives Claude a short brief of each project at the start of every session. Notes and tasks, prompt-time recall, a web viewer, and one shared server for all your machines if you want it.

## Install

The Pitwall installer sets it up (with the local model that fits your GPU) and keeps it updated:

```bash
curl -fsSL https://github.com/ParendumOU/pitwall-bootstrap/releases/latest/download/install.sh | bash
```

```powershell
irm https://github.com/ParendumOU/pitwall-bootstrap/releases/latest/download/install.ps1 | iex
```

By hand: download `pitwall-mem-<version>.tar.gz` from a release, check it against `SHA256SUMS`, unpack it, then add the folder as a Claude Code plugin marketplace and install the plugin: `claude plugin marketplace add <folder>` and `claude plugin install pitwall-mem@pitwall-mem`. It needs Node.js 22.13 or newer.

## More

Website: https://pitwall.parendum.com

License: MIT (see [LICENSE](LICENSE)). Each release includes its full source.
