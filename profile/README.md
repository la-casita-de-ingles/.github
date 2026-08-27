# La Casita de Inglés

An English academy for children aged 1 to 12 — **22 centres across Madrid, Barcelona,
Valencia and Vigo, plus classes online** — and the small team that builds the software it
runs on.

Everything here is written by that team: the platform families and staff use every day,
the site the school shows the world, the infrastructure underneath it, and the
documentation that keeps the four talking to each other.

## What we build

| | |
|---|---|
| **The platform API** | Enrolments, groups, schedules, billing and payments. Node.js · TypeScript · Express · PostgreSQL · Sequelize, with Redsys for card payments |
| **The backoffice** | The screens the school actually runs on — enrolment, groups, invoicing, staff records. Angular with signals and a design system of its own |
| **The public site** | Astro, built for accessibility and Core Web Vitals, with an agent that helps keep the content current |
| **The infrastructure** | Ubuntu, nginx, Docker, DNS, and the runbooks that make a server reproducible rather than remembered |
| **The deploy system** | OIDC-authenticated deployments from GitHub Actions, with no long-lived credentials on any machine |
| **The shared documentation** | Where the repositories talk to each other, and the only place a cross-team decision is allowed to live |

## How we work

The interesting part is not the stack. It is that a platform split across several
repositories, worked on by small teams and by AI agents, stays coherent — and that is a
documentation problem before it is an engineering one.

**A decision that crosses a repository is written down, or it did not happen.** Not in a
chat, not in a pull request comment. Each repository owns its own folder and nobody edits
anybody else's; when one team needs something from another, it opens a thread, and the
answer arrives in the same place. The record of what changed is append-only: entries are
never revised, and a later one supersedes an earlier one, the way commits do.

**Rules are barriers, not requests.** A convention that relies on everybody remembering it
is a convention that has already started to drift, so ours are checked mechanically — the
structure, the frontmatter, the boundaries, the links. Most of those checks exist because
somebody used the system, something broke, and they wrote up what happened instead of
quietly working around it. That last habit is the one we would keep if we could only keep
one.

**We write down why, not only what.** The reasoning behind a decision is the half that
disappears first and the half a future reader actually needs — including the options that
were considered and rejected, so the same argument is not had twice.

## The repositories are private

Deliberately. They carry the data and the operational detail of a school full of
children, and there is no version of that which is safe to publish. What is public is this
page.

<sub>[lacasitadeingles.com](https://lacasitadeingles.com)</sub>
