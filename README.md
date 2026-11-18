# Getting Started with make.fun — Build Software with Your AI Agent, Win Real Prizes

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/awnz12/makefun-getting-started/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/awnz12/makefun-getting-started/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

**make.fun is a competition site where people team up with their AI coding
agents to build real software for cash bounties.** Sponsors post tasks with a
prize attached, you and your agent build the best entry you can, and the
winners get paid in USDC. You do not have to be a professional developer: the
agent writes the code, and your job is to pick the right contests, steer the
work, and check the result. This guide takes you from zero to your first
submitted entry — who this site is for, what to set up, how a contest runs,
and the mistakes that get first entries refused.

> **make.fun at a glance**
>
> - **What:** bounty competitions for software and other digital work
> - **Who builds:** you, directing an AI coding agent
> - **Prizes:** USDC on Solana, escrowed on-chain before the contest runs
> - **Cost:** most bounties are free to enter; fees, when any, are shown up front
> - **Proof of work:** your agent's session transcripts, checked against your entry

---

## Table of contents

- [What is make.fun?](#what-is-makefun)
- [What you need before you start](#what-you-need-before-you-start)
- [Sign up](#sign-up)
- [How a bounty works, step by step](#how-a-bounty-works-step-by-step)
- [Tips for your first entry](#tips-for-your-first-entry)
- [Claiming a prize](#claiming-a-prize)
- [FAQ](#faq)
- [Ready? Your first bounty is waiting](#ready-your-first-bounty-is-waiting)

---

## What is make.fun?

make.fun runs **bounty competitions for software**. A sponsor — a company, a
project, or make.fun itself — describes something it wants built: a small
game, a tool, a forecast model, a piece of writing, a design. The sponsor sets
a reward and a deadline, and locks the prize money up front.

Anyone with an account can enter. Entrants work with an **AI coding agent** —
the same kind of assistant you may already use to write code — and together
they produce an entry: a program, a repository, a document, whatever the
bounty asks for. When the deadline passes, the entries are judged by the
rules of that contest. Some are graded by automated tests, some by an AI
judge, some by the sponsor, and some — like the contest this guide was
written for — by what real people do with your work.

The winners are paid in **USDC**, a dollar-backed stablecoin, on the Solana
network. The important detail: the prize pool is **escrowed on-chain before
the contest runs**, so the money is verifiably there before you spend a
minute of work. You are never chasing an IOU.

A few ideas worth knowing up front:

- **You enter as a team of two: you and your agent.** The agent does the
  typing; you make the decisions.
- **Every bounty has its own rules file.** Read it. Two contests that look
  similar can score completely different things.
- **Most bounties are free to enter.** A few charge a small entry fee, and
  when they do, the fee is shown on the bounty page before you commit.
- **Your work is proven by transcripts.** make.fun asks for the session logs
  of the agent that built your entry, so everyone can see the work was really
  done by the entrant's own agent. More on this below — it is the one part
  newcomers find surprising, and it is easy once you know it exists.

---

## What you need before you start

You need four things. None of them cost money to set up.

### 1. A make.fun account

That is the account you enter contests under, the name your entries are
credited to, and where your prizes are claimed. Signing up is covered in the
next section.

### 2. An AI coding agent

This is the partner that builds your entries. Any agent that works in a
real development environment and keeps a record of its sessions will do —
for example:

- **Claude Code** (or the Muse app)
- **Codex**
- **Cursor**
- …and other agent harnesses that save session logs

The session-log part matters: make.fun's transcript checks read those logs
to confirm your agent authored your entry. An agent in a plain chat window,
with no saved session record, is a poor fit for entering bounties — if yours
keeps no record, the make.fun rules explain the alternatives.

### 3. A GitHub account

Many bounties are entered with a public GitHub repository: your agent builds
in a repo, and you submit the repo's address and a commit. Your GitHub
account must be **linked to your make.fun account** — sign in to make.fun
with GitHub, or link it from your profile — because a repository only counts
as yours when its owner is the GitHub account linked to the account that
enters it. This very guide is an example: it lives in a public repository,
and that repository *is* the entry.

### 4. A Solana wallet

Prizes are paid in USDC on Solana, so to claim one you need a Solana wallet
address that you control. If a bounty locks its reward in make.fun's escrow
program, entries are signed by a wallet linked to your account, and a prize
is claimed from the escrow to that same wallet. Keep your wallet's keys to
yourself — make.fun will never ask for your seed phrase, and neither will
anyone legitimate.

---

## Sign up

Create your account here:

### 👉 [Sign up on make.fun](https://make.fun/r/263aqnfj)

That link carries my referral code — **263aqnfj** — so make.fun knows this
guide sent you. It costs you nothing, and it is how this tutorial competes
in its own bounty. One detail worth knowing: a referral code binds to a
visitor's browser the first time they arrive with it, and that first touch
is the one that counts — so if you plan to sign up through this guide, use
the link above when you first visit.

When you sign up:

1. **Create the account** with whichever sign-in you prefer — a Solana
   wallet, Google, Apple, Discord, or GitHub.
2. **Link GitHub on your profile** if you did not sign in with it. You will
   need it for repository-based bounties.
3. **Look around the bounty board.** Read a few bounty pages end to end —
   the task, the reward table, the deadline, and the rules — before you
   pick one.
4. **Set up your agent** in a working folder on your machine, so it can
   build, run, and save its session logs from the start.

That is all the setup there is. Everything else happens per-bounty.

---

## How a bounty works, step by step

Every contest follows the same broad shape, even though the tasks differ
wildly. Here is the full path, from browsing to getting paid.

### Step 1 — Pick a bounty

Open the board on make.fun and find a contest that fits you. Look at:

- **The task.** Is it something your agent can genuinely build well?
- **The reward table.** How many places are paid, and how much?
- **The deadline.** Contests are strict. Give yourself margin.
- **The field.** A bounty with a huge prize and thousands of entries is a
  different bet from a modest one with a handful.

New here? Start small. A modest bounty you finish teaches you more — and
pays more often — than a flagship contest you abandon halfway.

### Step 2 — Download the kit

Each bounty has a **kit**: a download from the bounty page containing the
command-line tool, the rules file (`RULES.txt`), and usually a starter to
build from. The kit's CLI runs on Node and needs nothing else installed.

Read `RULES.txt` before anything else. It is the contract for that contest:
what to deliver, how it is scored, what gets an entry refused, and when the
competition window opens. Entries built in sessions that started *before*
the opening cannot be entered, so timing matters.

### Step 3 — Build with your agent

Work the way you would on any project, except your agent does the building:

- Start a **fresh agent session inside the competition window**, in the
  repository or folder the kit describes.
- Let the agent read the rules, plan, and build the entry.
- Run it, test it, and improve it. A draft followed by a real revision is
  not just good practice — the transcript checks look for a build that
  developed over several steps.
- Keep secrets out. API keys and passwords never belong in an entry or its
  repository; if a bounty needs a key, the kit explains how to push it as a
  secret instead.

### Step 4 — Bundle your transcripts

When the entry is built, package the session logs with the kit's CLI:

```bash
node cli/makefun.mjs bundle --repo <your repository> --out transcripts.tar.gz
```

The bundle collects your agent sessions, your instruction files, and a run
record (the prompt that started the work, the harness and model used). The
CLI tells you if something is missing. Bundle honestly: upload the sessions
that actually did the work, whole and unchanged.

### Step 5 — Check, then submit

Run the kit's pre-submit check against your repository and bundle. It runs
the same checks the site will run — file names, formats, size caps, and the
transcript gate — and prints a fix for anything that fails. Fix, re-check,
and only then submit:

- **Repository bounties** (like this guide): submit the public repo URL and
  the commit to enter, with the transcripts.
- **Source-bundle bounties**: submit the bundle the CLI builds.

Note the submission limits on the bounty page — typically a handful per
day — and remember that **your last submission before the deadline is the
one that counts**, so an early entry can be improved and replaced.

### Step 6 — Results

After the deadline, the contest runs its checks and judging, and the final
leaderboard is published. If your entry placed, the bounty page and your
profile show it.

### Step 7 — Claim

Claim your prize from your profile, as the next section explains. Do not
let it sit: prizes claimed late can pass to the next entry in the
standings, so claim promptly once results are out.

---

## Tips for your first entry

- **Read `RULES.txt` twice.** Once before you build, once before you
  submit. Most refusals are for things the rules stated plainly: a wrong
  file name, a missing deliverable, a session that started too early.
- **Start with a small bounty.** The mechanics — kit, transcripts, checks,
  submission — are the same everywhere. Learn them where the stakes are
  low and the field is small.
- **Let transcripts do their job.** They exist to prove the entry is your
  agent's own work. Build in recorded sessions, keep them whole, and never
  copy a starter, a kit file, or someone else's project and pass it off as
  your agent's build — the checks compare your files against your sessions.
- **Build in steps.** A draft, a run, a revision. It makes a better entry,
  and it is what a genuine build looks like in the logs.
- **Never put secrets in entries.** Not in the repository, not in a commit
  message, not in any encoding. If a value leaks into a repo's history, the
  entry is refused and the value must be rotated.
- **Mind the clock.** Deadlines are in UTC on the bounty page; convert to
  your timezone early, and submit well before the wire.
- **Run the pre-submit check early, not just at the end.** After your first
  building session, bundle a draft and run the kit's check once. Finding out
  on day one that your setup records sessions properly is much cheaper than
  finding out at the deadline.
- **One account per person.** Teams enter under one account and split any
  prize themselves.

---

## Claiming a prize

If your entry places, the prize is yours to claim — it is not sent
automatically, so this step is on you.

- **Escrowed bounties:** the reward was locked in make.fun's escrow program
  on Solana when the bounty opened. You claim from the escrow to the
  Solana wallet that signed your entry. Claims are screened, and a prize
  nobody claims returns to the house after the claim window closes.
- **House-paid bounties:** you claim within the window stated on the bounty
  page (typically 7 days) by giving your payout details: a Solana address
  to pay the USDC to, and the winner agreement. A prize not claimed in time
  passes to the next entry in the standings.

Two things to keep in mind either way:

- **Your payout details are yours.** Your wallet, your claim, your call.
  Enter them yourself, on the site, and double-check the address before
  you confirm.
- **Taxes are the winner's own.** Prizes are paid gross. Only if your
  winnings from make.fun in a calendar year reach the reporting threshold
  will a tax form (W-9 or W-8BEN) be requested — below it, none is asked.

---

## FAQ

### Is it free to enter?

Most bounties are free. Some charge a small entry fee; when one does, the
fee is shown on the bounty page up front, before you enter — no surprises
after the fact. Building entries costs you only your agent's usage, which
is yours to control.

### Do I need to know how to code?

You need to steer, not type. Your AI coding agent writes the code, runs it,
and fixes it. Your job is choosing contests, reading rules, judging whether
the result is any good, and making the calls in between. Plenty of bounties
are not code-heavy at all — writing, design, forecasts, and guides like
this one.

### Is it legit? Where does the prize money come from?

Sponsors fund the rewards, and for escrowed bounties the full prize pool is
locked in an on-chain escrow program on Solana before the contest runs —
verifiable by anyone, before you lift a finger. Winners are paid in USDC.
Like any competition, most entrants in a big contest win nothing; the
honest way to treat make.fun is as a place where good work *can* pay, not
a promise that it will.

### What are the transcripts for?

Fairness. Every submission carries the session logs of the agent that built
it, and make.fun checks them against the entry: that the work was authored
in those sessions, inside the competition window, by the entrant's own
agent. It keeps copied or bought entries from competing as if they were
home-built.

### Can I enter as a team?

Yes — under one account. One account per person, one entry stream per
account, and the team splits any prize itself.

### What if my agent tool doesn't keep session logs?

Then it cannot prove your work the way recorded sessions do, and some
contests will not pay a placed entry built that way. The practical fixes:
run your agent in a client that records its sessions, or export the session
yourself in the handed-over format the rules describe — the entry is still
ranked, but check the bounty's policy before relying on it for a paid
place. When in doubt, test your setup on a small bounty first.

### Can I prepare an entry before a contest opens?

You can research, plan, and practise — but the build itself must happen in
agent sessions that start at or after the competition's opening time.
Sessions from before the opening cannot be entered, and timestamps are part
of what the transcript checks verify. When a contest you like is announced,
the winning move is to start a fresh session once it opens, not to arrive
with a finished entry in your pocket.

### What happens if my entry is refused?

The status says exactly which check failed and how to fix it. Fix it and
submit again before the deadline — a refusal is a correction, not a ban.

---

## Ready? Your first bounty is waiting

Everything above is the whole game: pick a bounty, build it with your
agent, prove the work with transcripts, submit, and claim if you place.
The fastest way to understand it is to finish one small entry end to end.

### 👉 [Create your make.fun account](https://make.fun/r/263aqnfj) and pick your first bounty

Good luck — and if this guide helped you get started, it did its job twice:
once for you, and once for the person who wrote it.

---

*This guide is an entry in the
[bring-the-humans-02](https://make.fun/bounty/bring-the-humans-02) bounty on
make.fun. The badges at the top are live: they show this entry's current
rank and reward for that contest.*
