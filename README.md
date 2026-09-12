# Privacy Removal

A Codex skill for finding your exposed home and email addresses, submitting authorized removal requests, and tracking what actually disappears.

It covers Google and Bing search results, people-search opt-outs, verification email handling, manual support fallbacks, and a private removal tracker. Provider-specific instructions are starting points that must be checked against the current official service.

## Install

Copy [`skills/privacy-removal`](skills/privacy-removal) into your Codex skills directory, usually `~/.codex/skills`. If a skill with that name already exists, review it before replacing it.

Invoke it with:

```text
Use $privacy-removal to find my exposed home and email addresses and manage removal requests.
```

Provide identity details privately in your own session. The skill uses the available browser/search tools and, when authorized, an email connection. Some services require you to sign in or complete verification yourself.

## What it keeps separate

- Confirmed identity details, uncertain matches, and rejected associations.
- Email addresses being searched and the address receiving provider replies.
- Source-site suppression and search-engine delisting.
- Request submission, provider approval, and verified disappearance.

Search coverage and outcomes are recorded explicitly. The skill does not promise complete removal from the internet or assume every listing qualifies for removal. Public email searches do not establish whether an address is in a data breach.

## Files

- [`SKILL.md`](skills/privacy-removal/SKILL.md): core workflow and decision rules.
- [`references/services.md`](skills/privacy-removal/references/services.md): official provider routes and form-specific details.
- [`assets/removal-tracker.md`](skills/privacy-removal/assets/removal-tracker.md): blank template to copy into a private case directory.

This repository contains reusable instructions and a blank template. Keep completed trackers, evidence screenshots, email contents, profile URLs, and verification links outside it. No actual case records are bundled.
