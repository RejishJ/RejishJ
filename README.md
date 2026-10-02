# Rejish J

**I build tools that work offline, keep your data where you can see it, and never ask you to make an account.**

AI & Data Science student · Coimbatore, Tamil Nadu, India · open to relevant opportunities

[Portfolio](https://rejish-portfolio.vercel.app) → [GitHub](https://github.com/RejishJ) → [LinkedIn](https://www.linkedin.com/in/rejishjd)

---

I open a terminal first and a browser second. Most of what I make starts as
something I wanted at a prompt: a cheat sheet I could actually *run*, a better
way to read a repository's history, an AI feature that keeps working when the
network drops. Python is home base. Linux is the office.

---

## Work

### [cheat-cli](https://github.com/RejishJ/cheat-cli)

*A cheat sheet for your terminal — searchable, editable, runnable.*

Every developer keeps a file of commands they can never quite remember.
cheat-cli turns that file into a real tool: entries live in a plain CSV you can
read and version yourself, AI suggestions run through local Ollama or any
OpenAI-compatible endpoint, and `--offline` means the whole thing works with no
network at all.

The detail I like most: you can execute an entry straight from the TUI,
and a deterministic classifier stops you first when a command looks like
`rm -rf`, `dd`, `mkfs`, or `sudo` — it lists why, then asks. The docstring
doesn't oversell it either: *a confirmation policy, not a sandbox*.

```console
$ cheat search docker
tool    command                           description                          tags
------  --------------------------------  -----------------------------------  ---------------
docker  docker ps                         List running containers              containers list
docker  docker compose up -d              Start services in detached mode      services start
docker  docker compose logs -f            Follow service logs                  logs debug
docker  docker exec -it <container> bash  Open shell in running container      shell access
docker  docker system prune -a            Remove unused containers and images  cleanup space
docker  docker images                     List docker images                   images list
docker  docker volume ls                  List docker volumes                  volumes list
```

`pip install cheat-cli` · [PyPI](https://pypi.org/project/cheat-cli/) · [Releases](https://github.com/RejishJ/cheat-cli/releases) · MIT · CI on 3.9–3.12

### [backintheday](https://github.com/RejishJ/daily-dev/tree/main/backintheday)

*Git history, asked better questions than "what happened recently."*

`git log` answers "what changed last week". The questions I actually had are
bigger — how activity spread across a project's whole life, how one file
drifted, how two eras of development compare. backintheday builds those
higher-level views on raw git output, entirely on your own machine.

Two decisions I'd defend in review: it shells out to the `git` CLI instead of
taking a library dependency, and runtime stays standard-library-only. Both are
written up as ADRs. The tests manufacture whole temporary repositories with
real commits to run against. It ships one command today — `history` — and says
so plainly rather than implying the rest.

[source — nested in `daily-dev`](https://github.com/RejishJ/daily-dev/tree/main/backintheday)

### [autospare-marketplace](https://github.com/RejishJ/autospare-marketplace)

*Two Flutter apps over one Firebase backend, because a shop owner and a
customer never want the same screen.*

The interesting part wasn't the app — it was serving one inventory to two
audiences with different rights: customers browse, filter by condition and
track orders; the shop manages products, stock, and analytics. Provider and
Riverpod over Firestore, Auth, and Storage.

Honest status: early, rough in places, and the repository says exactly that.

---

## How I build

- **Boundaries are load-bearing.** Interface, service, and storage stay
  separate layers; the storage backend should be swappable without rewriting
  what sits above it.
- **Tests should make their own worlds.** Temporary git repositories, offline
  paths, destructive-action confirmations — behavior, not the implementation
  details behind it.
- **Local first, account never.** Files you can read, no sign-up wall, network
  optional. An AI feature is an addition, not a dependency.
- **Ship it like you mean it.** CI on every change, tagged releases with a
  changelog, and security and contributing docs written before anyone asks.

---

## Now

**Building** — more of the same on purpose: command-line tools that stay fast,
local, and account-free. Most of the effort goes into cheat-cli's next
iteration.

**Learning** — machine learning in depth alongside my degree, then security,
operating systems, and hardware — the territory where you can't hand-wave.
Learning it the only way I know how: build it small, break it, fix it.

---

## Elsewhere

[Portfolio](https://rejish-portfolio.vercel.app) · [GitHub](https://github.com/RejishJ) · [LinkedIn](https://www.linkedin.com/in/rejishjd) · [rejish.j.d@gmail.com](mailto:rejish.j.d@gmail.com)

Everything here is public — open the source. It explains itself better than
this page can.
