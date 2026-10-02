# Rejish J

AI & Data Science student building practical, local-first developer tools in Python.

Coimbatore, Tamil Nadu, India · open to relevant opportunities

---

## Selected work

### cheat-cli

A terminal-first cheat sheet for people who live in the shell: search, add, and
run your own command references without leaving the terminal. The data is a
plain file on your machine, and everything except the optional AI suggestions
works with no network at all.

- **Local by default** — no account and no service behind it; your notes stay in
  a file you can read, edit, and version yourself.
- **Optional AI** — suggestions can run against local Ollama or any
  OpenAI-compatible endpoint, and there is a genuine offline mode when nothing
  is reachable.
- **Replaceable underneath** — storage sits behind a small interface, so the CSV
  backend is an implementation choice rather than the shape of the application.
- **Released like a package** — `pip install cheat-cli` (MIT, current release
  0.1.3), tagged releases, and CI running ruff, the tests, and a build check
  across Python 3.9–3.12. The suite is 23 test modules covering the CLI, the
  TUI, storage, safety, and offline behavior.

[Source](https://github.com/RejishJ/cheat-cli) · [PyPI](https://pypi.org/project/cheat-cli/) · [Releases](https://github.com/RejishJ/cheat-cli/releases)

### backintheday

A command-line tool for exploring how a Git repository evolved over time.
`git log` answers what happened recently; this is aimed at the harder questions
about a project's whole past — how activity was distributed, how a file changed,
how two periods of development differ.

Zero runtime dependencies, a layered structure that further commands are meant
to sit on, architecture decision records for the trade-offs, and tests that
build temporary Git repositories rather than touching real ones. It does one
command today and says so plainly instead of implying the rest.

[source — nested in `daily-dev`](https://github.com/RejishJ/daily-dev/tree/main/backintheday)

### autospare-marketplace

An early-stage Flutter marketplace for vehicle spare parts: a customer app and a
separate admin app, both backed by Firebase. Two apps over one backend meant
solving state and sync for two different audiences rather than one.

---

## How I work

- **Keep the seams visible.** Interface, service, and storage stay separate
  layers; nothing skips one to reach another, and the storage backend can be
  replaced without rewriting what sits above it.
- **Test the behavior that matters.** Suites that spin up real temporary Git
  repositories, exercise the offline path, and check that destructive actions
  ask first — not just the happy path.
- **Default to local.** Files over services, no account requirement, network
  optional. An AI feature should be an addition, never a dependency.
- **Ship on purpose.** CI on every change, versioned releases with a changelog,
  and security and contributing documents written before anyone asks for them.

---

## Right now

**Building** — small, dependency-light command-line tools in the same family as
`cheat-cli`: local data, clear layers, no account. Software meant to stay useful
for years rather than demos that need a server.

**Learning** — AI and machine learning in depth alongside my degree, plus
security, OS internals, and hardware. Coursework and side projects so far, and
the part I like is how much they share with the tooling above.

---

## Elsewhere

[Portfolio](https://rejish-portfolio.vercel.app) ·
[GitHub](https://github.com/RejishJ) ·
[LinkedIn](https://www.linkedin.com/in/rejishjd) ·
[rejish.j.d@gmail.com](mailto:rejish.j.d@gmail.com)

This README is the short version; the repositories carry the detail, and the
portfolio carries the rest.
