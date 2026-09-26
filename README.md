# Rejish J

I build **local-first developer tools in Python** — terminal software that
keeps your data on your machine and works without a network.

---

### Selected work

**[cheat-cli](https://github.com/RejishJ/cheat-cli)** — a terminal-first cheat sheet
Search, add, and run your own command references from the terminal: a Textual
TUI, optional AI suggestions (local Ollama or OpenAI-compatible, with a real
offline mode), and a data layer defined by a `StorageBackend` protocol.

`pip install cheat-cli` · [PyPI](https://pypi.org/project/cheat-cli/) · MIT

**Where the engineering is:**

- `cheat_cli/core/` — storage contract (`load/save/add/update/delete`) kept
  separate from the CSV implementation
- `tests/` — 23 modules covering CLI, TUI, storage, safety, offline behavior
- `.github/workflows/ci.yml` — ruff + tests on Python 3.9–3.12 + package
  build validation on every PR
- `CHANGELOG.md`, `SECURITY.md`, `CONTRIBUTING.md` — releases are tagged and
  documented

---

### Currently building

- **cheat-cli** — next iteration of the storage layer
- **SecureChain** — blockchain identity & asset platform (Solidity,
  TypeScript, React), from Smart India Hackathon 2026.
  *In progress — not public yet.*

---

### How I work

- Layer boundaries first: CLI/TUI → service → storage, nothing skipping layers
- Tests describe behavior, not implementation details
- Changes go through CI; releases are tagged with a changelog
- Prefer software that works offline, keeps data local, and doesn't require an account.

---

### Contact

[Portfolio](https://rejish-portfolio.vercel.app) ·
[LinkedIn](https://www.linkedin.com/in/rejishjd) ·
[rejish.j.d@gmail.com](mailto:rejish.j.d@gmail.com)
