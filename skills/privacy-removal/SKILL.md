---
name: privacy-removal
description: Find a user's exposed home addresses, email addresses, and phone numbers on Google, Bing, and people-search sites; carry out authorized opt-outs and track removal decisions. Use for self-directed privacy cleanup or an explicitly authorized representative, not background checks on unrelated people.
---

# Personal information removal

Turn a privacy cleanup request into a private record of verified matches, authorized requests, and independently checked outcomes. Search engines and source websites require separate actions; a submitted request is not a completed removal.

## Establish scope without restarting the conversation

Reuse the user's confirmed identity details, chosen verification email, corrections, and existing approvals. Distinguish a request to inspect exposure from authorization to submit removals or contact a provider. Carry out actions already authorized; do not ask the same permission again simply because a form has another step.

Ask only for information that blocks the next useful action. Usually a name plus a confirmed city, former address, or email address is enough to begin. Collect a birthdate or other additional identifier only when an official opt-out flow actually requires it and the user elects to provide it. Allow the user to enter sensitive details themselves. Do not infer citizenship, current residence, legal eligibility, threats, or a court order from a search result.

Keep three distinct identity sets:

- User-confirmed names, residential addresses, email addresses, and phone numbers, including former ones.
- Newly discovered associations that still need confirmation.
- Associations the user has explicitly rejected.

Never turn a rejected address, possible relative, unconfirmed apartment number, or similar email address into an asserted identity fact. A removal request can target an otherwise well-matched profile without affirming every claim it contains.

## Keep case data private

Copy [the blank tracker](assets/removal-tracker.md) to a private case directory outside the skill and any published repository. Follow the user's workspace conventions. Use owner-only file permissions where supported. Keep actual names, addresses, phone numbers, email messages, screenshots, profile URLs, and report identifiers in that private case, not in the reusable skill.

Record which fields a provider required without saving raw birthdates, identity-document contents, credentials, or verification tokens. Retain only the evidence needed to identify a result and verify the requested outcome. Public examples must use synthetic placeholders.

## Find and qualify exposure

Use the user's requested browser and search engine. Otherwise use available search tools; use a connected browser for interactive forms. Follow the environment's browser skill before browser interaction. An email connector is useful for scoped verification and decision messages when access is available and authorized.

Search names with confirmed addresses individually. Compare quoted and unquoted variants when useful: engines sometimes omit terms or return different results for the same information. Google and Bing need separate checks; a clean result on one does not establish absence on the other. Record the engine, query, date, and extent inspected.

Match the name and a distinguishing confirmed detail in the result or source page. Treat a name alone, an address-only property listing, a different unit in the same building, or a relative's record as insufficient evidence. Do not expand into investigating other people. Ask the user to confirm newly found addresses before adding them to the confirmed list.

Capture the exact target URL and minimal supporting evidence. Preserve record IDs and meaningful query parameters. Distinguish source-page evidence from search snippets; a blocked source visit is not evidence that the page is absent. Stop broadening a search when it no longer adds useful evidence, and state the bounds checked.

### Email exposure checks

Use the email addresses the user has selected for exposure checks. Keep that list distinct from the email chosen to receive opt-out confirmations and from the account attached to an email connector. Do not infer additional addresses from the inbox.

Search each complete email address in quotes on the requested engines, then combine it with the confirmed name when useful. If an engine omits terms or treats punctuation unexpectedly, inspect an unquoted variant. Do not assume the same local part on a different domain, an inferred alias, or an obfuscated address belongs to the user without confirmation.

Record the exact page URL, whether the full email is visible, its surrounding identity context, and whether the evidence is a snippet or source page. A page exposing the confirmed full address can be a match even without a name. For a removal request, select the email/contact-information category and supply the address as published. Add email monitoring only when requested and supported by the current provider; verify saved settings rather than assuming capacity or coverage.

Search-engine checks do not establish whether an address is in a data breach. Breach monitoring is a separate, user-requested scope; never request passwords, test logins, send probe emails, or trigger account-recovery messages to investigate exposure.

### Phone exposure checks

Use only phone numbers the user has confirmed and selected for exposure checks. Keep these separate from a number used for provider verification. Record an explicit country calling code; derive one only from a user-confirmed country for that number. If it remains ambiguous, search the supplied form and ask before generating international variants.

Search the exact supplied format in quotes on the requested engines, then useful international, digits-only, and spaced variants; include familiar parentheses or hyphen formatting when relevant. Preserve significant digits and use the confirmed country's numbering conventions when changing prefixes. Combine variants with the confirmed name when useful. Record the query and bounds checked; do not generate neighboring numbers or infer other numbers from a matching profile.

Verify the number and its surrounding name or identity context before targeting a profile. Numbers can be shared or reassigned: a matching number alone does not establish that another person's record belongs to the user. Distinguish current, former, and shared numbers, ask about ambiguous associations, and avoid affirming unrelated profile details. Record whether the full number is visible and whether the evidence is a search snippet or source page.

For an authorized removal, select the phone/contact-information category and supply the number as published with the exact target URL. Do not seek duplicate permission for an action already authorized. Phone monitoring requires the user's request and support in the current provider. Public search results do not establish a data breach; do not call, text, test logins, or trigger account-recovery probes to investigate exposure or ownership.

## Carry out authorized removals

Read [provider routes](references/services.md) only for the services in the case, then verify the current official form and requirements. Provider interfaces, covered brands, limits, and turnaround estimates can change.

For each confirmed match:

1. Check the tracker and relevant receipts for an existing request before creating another.
2. Select the appropriate source opt-out or search-engine privacy-removal route. Use an outdated-content tool only when the source was actually removed or changed and the tool's criteria fit.
3. Supply the minimum truthful details. Use the chosen verification email; do not silently substitute the connected mailbox's address. If sending from a different account is necessary, disclose the difference and stay within the user's authorization. Accept terms or make attestations only with the authorization required by the active tools and the user's existing consent.
4. If correct identity details find no record, use an official manual-support route when available. Do not invent a matching birthdate or change the user's legal name to force a result. Explain the mismatch and provide the exact matched URL.
5. Capture the receipt, case ID, target URL, time, and stated review window. A success screen establishes submission; approval and verified disappearance are separate states.

For verification links, check sender, intended provider, recipient, and expiry. Do not expose or persist tokens. When an email field is omitted from a text snapshot, inspect the visible form if needed before assuming it is empty. After a detached or timed-out submission, inspect the page and receipts before retrying; the action may have succeeded.

Browser site-safety denials, blocked verification links, authentication, and human-verification puzzles require the handoff prescribed by the active tool. Do not retry a denied action through another browser, raw HTTP, decoded tracking links, or another agent. A search-engine removal report based on already observed indexed evidence may remain a distinct permitted action. Do not generalize a session's blocked domains into a permanent blacklist.

## Verify and report progress

Track source suppression and search visibility independently. Useful states are: identified, needs identity confirmation, ready, verification needed, submitted, approved, rejected, and disappearance verified. Attach a timestamp and evidence to each state change.

Read provider decisions before scheduling follow-ups or sending duplicates. Recheck approved URLs after the stated propagation window. Keep the original query and note which engine and query were checked; a missing result does not prove universal or worldwide removal. New profile URLs generally need their own request.

Report what was found, what was actually submitted, any decisions received, and what still requires the user or provider. Include the private tracker link when useful. Set up recurring checks only if requested; a recorded follow-up date is not a scheduled automation.
