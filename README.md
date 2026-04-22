# Ghostnote Labs — Legal

Public-facing legal documents for Ghostnote Labs LLC products.

Hosted at: **https://ghostnote-labs.github.io/legal/**

## What's here

- [`privacy.md`](privacy.md) — Privacy policy. Served at `/privacy`.
- [`terms.md`](terms.md) — Terms of service. Served at `/terms`.
- [`index.md`](index.md) — Landing page at `/`.

## Publishing workflow — IMPORTANT

**This repo is public, and GitHub Pages builds everything here into an indexable site.** Product codenames (e.g. `Numen`, `Ember`) must NOT appear in the hosted files until the underlying trademark clearance is complete — see `docs/LEGAL.md` Priority 1 in the private product repo.

Canonical sources live in the **private** product repo at `eSmelser/numen` → `docs/legal/`. Those files may use the product name freely for developer clarity.

### When pulling a policy change from the private repo into this public one:

1. Start from the canonical markdown file in `eSmelser/numen/docs/legal/`.
2. Replace every product-specific codename with a generic placeholder:
   - `Numen` → `the App` or `our mobile application`
   - `Ember` (familiar's name) → `the AI familiar` or `characters`
   - Any other unreleased proper noun → generic equivalent
3. Prepend the Jekyll frontmatter block (`---\nlayout: default\ntitle: ...\npermalink: /...\n---`).
4. Commit + push to `main`. Pages rebuilds within ~1 minute.

### When to restore product names

Once the trademark for the product is filed and cleared (or at public announcement at the latest), update the hosted version to use the real name. Until then: generic placeholders only.

## Theme

Jekyll with the built-in Cayman theme. No custom styling. Minimal by design — legal docs are for reading, not decoration.

## Update cadence

Policies are versioned by the "Effective date:" line at the top of each document. When substantively changing a policy in production, bump the date and archive the prior version in a git tag so historical records are retrievable.
