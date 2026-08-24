# Lede

Lede is a personal dev and tech news page. Once a night it reads a set of feeds, drops what you've said you don't want, summarises and grades what's left against your own written interest profile, and publishes a single page for you to read in the morning.

Open it at **https://mgreuel.github.io/lede/**.

![The Lede front page](docs/screenshot.png)

The page is a **desk**: a rail down the left that never moves, and one list of articles scrolling beside it.

1. **The rail.** Everything that narrows or reorders the list, still there on the twentieth screen of scrolling. It carries the app's name and **Settings**; when the data is from — "Data as of 20:36, 19 Aug 2026", always the full instant, so you can judge for yourself how old a run is rather than being told; the four orders; the way back to what you've hidden; and the fold over what the model set aside. Under the timestamp, on a night that didn't go to plan, one line says so and nothing more: what actually went wrong is a question for the private repository and the workflow log, not for a public page. A healthy night shows nothing at all, so the absence of that line is itself the statement that the run was fine. Nothing is ever pushed at you — no banners, no toasts to dismiss.
2. **The order.** Score, Date, Reaction or Topic. Press the one the list is already in and it reverses, so choosing an order and turning it round are one gesture rather than two controls.
3. **The list header.** How many articles you're looking at and which order they're in, stuck to the top while you scroll.
4. **The list.** Every article the filters leave, one after another, with nothing that stops to ask permission to continue. Each row carries its grade in a column at the left, the headline, its summary, where it came from, the date, and how much attention it's getting elsewhere. Grouped by topic, each heading says how many rows are under it and stays on screen while you're inside that group.
5. **The local-only notice.** Shown once, until you dismiss it, if your reading state is being kept in this browser alone. **Set up syncing** takes you straight to the settings panel, which opens at the top of the list.

## Reading the list

- A summary written for you is labelled **Summary generated**, so you always know whose words you're reading.
- An article that arrived with nothing but a headline is shown with no summary at all, rather than an invented one. You are never misled by a confabulation.
- A **Lifted** badge means an article was promoted a grade because it's being widely shared.
- Popularity is shown as raw numbers per source — Hacker News points and comments, how many feeds carried it, Bluesky likes — never as one blended score, so you can judge what kind of attention it got. *Never measured* looks different from *measured and ignored*: you never read silence as a verdict.
- The default order is your grade first, then how hard the world actually reacted to the article, then how new it is — so a thousand equally-graded articles are not in an arbitrary order. **Reaction** asks that second question first, if you'd rather go looking for what everyone is talking about than for what your profile says you want.
- The order is for this visit only — it isn't remembered, and reloading resets it.

## Read and dismissed

- Opening an article counts as reading it. There's no bookkeeping to do.
- Each row has a dismiss button for something graded too highly.
- Either way the row disappears at once and an undo toast appears at the bottom. A mis-tap costs nothing.
- Hidden is never lost. The rail's count and **Show hidden** bring them back.
- What the model rejected outright — a veto rule of yours, or a grade of nought — is out of the list but never dropped. **Show what the model set aside** in the rail says how many there are and puts them at the foot of the list, so a rule that matches too much is something you can find and fix.
- Three empty states, told apart: a genuinely quiet day, a day you've finished, and a night no run reported on. *No news* is never shown as *no run*.

## Reading state across devices

By default everything stays in this browser. No account, no setup, nothing to configure — trying the site costs nothing.

Turn on sync and your reading history follows you between machines, so you never triage the same article twice.

The articles are public, but what you read is nobody's business. So your reading history is kept in a private repository that belongs to you — not in this one, and not on any server of ours. There is no server; the site is a set of static files.

Sync needs two things: a private repository you own, and a fine-grained access token scoped to that one repository — narrower than a normal login, and pasted once. There's no login flow to sit through.

The settings panel walks you through both steps.

## Everywhere else

Light, dark and system colour schemes are all respected.

This is a desktop surface. The rail is permanent at every width the page supports, and there is no phone layout — that's a decision about the viewport and not about access: everything a hover tells you is also said in words, so nothing is reachable only by pointing at it.
