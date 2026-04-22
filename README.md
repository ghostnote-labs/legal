# Ghostnote Labs — Legal

Public-facing legal documents for Ghostnote Labs LLC products.

Hosted at: **https://ghostnote-labs.github.io/legal/**

## What's here

- [`privacy.md`](privacy.md) — Privacy policy. Served at `/privacy`.
- [`terms.md`](terms.md) — Terms of service. Served at `/terms`.
- [`index.md`](index.md) — Landing page at `/`.

## Publishing workflow — IMPORTANT

**This repo is public, and GitHub Pages builds everything here into an indexable site.** Any unreleased product codenames, character names, or other trademark-sensitive terms must NOT appear in this repo (including this README) until the underlying trademark clearance is complete.

Canonical source drafts live in the private product repository. Those files may use product-specific names freely for developer clarity.

### When pulling a policy change from the private source into this public repo:

1. Start from the canonical markdown file in the private product repo's `docs/legal/` directory.
2. Replace every unreleased product-specific name with a generic placeholder:
   - Product codename → `the App` or `our mobile application`
   - Any character or system name not yet publicly announced → generic equivalent (e.g. `the AI familiar`, `characters`, `game mechanics`)
3. Prepend the Jekyll frontmatter block (`---\nlayout: default\ntitle: ...\npermalink: /...\n---`).
4. Commit + push to `main`. Pages rebuilds within ~1 minute.

### When to restore product names

Once trademarks are filed and cleared (or at public announcement, whichever comes first), update the hosted version to use the real names. Until then: generic placeholders only — including in this README.

## Theme

Jekyll with the built-in Cayman theme. No custom styling. Minimal by design — legal docs are for reading, not decoration.

## Update cadence

Policies are versioned by the "Effective date:" line at the top of each document. When substantively changing a policy in production, bump the date and archive the prior version in a git tag so historical records are retrievable.
