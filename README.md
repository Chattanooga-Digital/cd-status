# Chattanooga.Digital — public progress board

A single static page showing what the co-op runs, what's in testing, what's planned, and what each
thing is waiting on. Served by GitHub Pages from this repository.

**Live:** https://tortoisewolfe.github.io/cd-status/

## Why this exists

A member-owned co-op should be legible to its members. Progress that only exists in a private issue
tracker isn't visible to the people the work is for.

## What belongs here, and what doesn't

This repository is **public**. The page is written so that it can be.

**Included:** services by what they do, public addresses, delivery stage, what each item is waiting
on, and how long it has been waiting.

**Deliberately excluded:** internal hostnames, container/stack identifiers, hosting-control-panel
details, infrastructure ownership, credential and backup mechanics, security-advisory identifiers
for anything unpatched, and anything relating to invoicing or private correspondence.

Those live in the internal operations record (`docs/OPERATIONS-MAP.md` in the main private
repository). **When updating this page, copy conclusions across by hand — never paste from the
internal map.** The two documents have different audiences on purpose.

## Editing

`index.html` is a single self-contained file: no build step, no dependencies, no external requests.
Edit it and push; GitHub Pages redeploys automatically.

It honours the visitor's light/dark preference and has a manual toggle that persists in
`localStorage`.

## Accuracy

Every status claim should be checked against the running systems before it goes in. An inaccurate
status board is worse than none — it converts "we don't know" into false confidence.
