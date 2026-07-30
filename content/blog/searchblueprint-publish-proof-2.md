---
title: "SearchBlueprint publish proof"
slug: "searchblueprint-publish-proof-2"
description: "Proof that an article published from SearchBlueprint becomes a reachable page."
keyword: "searchblueprint publish test"
date: "2026-07-30T15:23:50.870Z"
---
This page was committed by SearchBlueprint's GitHub adapter to prove the publish
round-trip end to end: commit, build, and a URL that actually resolves.

## Why this exists

A successful write is not a successful publish. Three publish events once recorded
`success` while the page 404'd, because the committed format did not match what the
site renders. This repo is the control.

## What was verified

| Step | Checked |
| --- | --- |
| Token scope | Contents read/write on one repo |
| Commit | File present on the live branch |
| Reachable | Public URL returns 200 |
