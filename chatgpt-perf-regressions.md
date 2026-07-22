## 2026-07-22 update: ##

People are still commenting on the post from three months ago. OpenAI has completely stopped replying over the bug. Like many of you I couldn't wait so I made my own chatlogging function. You can try it here :

https://chatgpt.com/g/g-6a3d7f2dad5481919ffb5c8b000c4a7d-mia

It logs each message and you can request the log anytime, .md or .html, you can even add the log to the semantic map (SM) for searching it alongside your other data.


## 2026-07-02 update: ##

After the user explicitly withdrew consent to automated handling and requested human escalation, OpenAI Support created a new case number, 10845775, and sent another automated response routing the issue to generic account export, uploaded-file deletion, and account deletion resources. The automated message also included a notice that support conversations may be used to improve OpenAI services, including models, if training is enabled. This strengthens the evidence of a support automation / case-routing failure separate from the original transcript access bug.


## 2026-06-13 update:

Another Reddit user reports the same ChatGPT preservation/export failure for weeks on Mac across every browser tested. They also report testing ChatGPT shared links in every browser with no success. This strengthens the evidence that the issue is not limited to one browser or ordinary local clipboard failure. The user describes major workflow harm and says people depend on chat contents for active working projects.
## 2026-06-12 update

Data-quality note: Chatbot-use records from early April 2026 onward may be sullied if users relied on browser-visible copy, print, save, search, or extension export paths for long ChatGPT conversations. Public evidence does not yet establish the exact rollout date, but multiple anchors point to early April 2026 as the current earliest warning window.

## 2026-06-01 update:

A new Reddit commenter reports the same transcript preservation failure in the ChatGPT Windows app. They say they previously used Ctrl+A / Ctrl+C, but as of yesterday could no longer do so. They reported the bug to OpenAI and have started manually saving each prompt, which is tedious and triggers repeated "too many requests" warning boxes even though the workflow continues. They also report considering extensions but agree that users should be able to export their work directly.

This adds the Windows app to the affected surface and strengthens the workflow-impact record: users are being pushed into manual prompt-by-prompt salvage, high click counts, warnings, and physical strain risk because no reliable per-conversation export exists.

## 2026-05-30 update:

A new Reddit commenter reports inspecting the frontend behaviour and says ChatGPT loads placeholders for portions of long threads, then reloads the relevant portion into the DOM as the user scrolls. They report that off-screen items are replaced by placeholders, so selecting from top to bottom can load and unload portions of the thread during selection, leaving large gaps in copy/paste or Print-to-PDF output.

The commenter says they have not found a way to block this behaviour. They describe a possible forensic workaround: use DevTools, cache network calls, reload, scroll slowly while waiting for each prompt/reply to load, export HAR, then try to reconstruct the thread or produce PDFs of subsections.

This supports the current bug model:

ChatGPT presents one conversation to the user, but browser-level operations may only access the mounted DOM slice or currently loaded transcript segments.

This also reinforces the product need:

- first-party per-conversation export
- full-transcript Archive / Print / Search mode
- warning when browser-level search/copy/print/save cannot access the full transcript
- no reliance on HAR reconstruction, DevTools, or user forensic extraction for ordinary archive use

The same commenter argues that users are not being told they cannot export stable records of their threads. Their legal characterization should be treated as their view, not as established fact, but the archive-integrity concern is directly relevant.

## 2026-06-01 update: r/ChatGPT post reports a 5000-node conversation where normal PDF export produced a blank result

A new r/ChatGPT post reports a 5000-node conversation where normal PDF export produced a blank result, an AI Exporter extension failed, archiving the chat before saving did not help, and Ctrl+S could not save the full conversation because the updated UI only loads visible content rather than the whole thread. This is another public report connecting PDF/export failure to transcript virtualization or visible-slice loading behavior.

## 2026-05-30 update: support case loop and missing diagnostic-material question

The issue remains active.

A third OpenAI Support case has now been created for the same ChatGPT Web transcript bug:

- Case 08747965
- Case 09120830
- Case 09371968

Case 08747965 was previously summarized by OpenAI Support as escalated to ChatGPT Web engineering.

However, later cases have continued to ask for the same user-supplied diagnostic material, including screenshots, screen recordings, and HAR files, rather than linking back to the existing Web engineering escalation.

The current support loop is:

1. User reports ChatGPT Web transcript access failure.
2. User gives browser, OS, repro steps, affected routes, and public cross-user reports.
3. Support asks for HAR, screenshot, or screen recording.
4. User points out that OpenAI can reproduce this internally with a test account and marker strings.
5. Support asks again for HAR and recording.
6. New case number is created.
7. Same request repeats.

This is now part of the issue.

The bug is not dependent on one user account, one private chat, or one browser. Reports now cover ordinary desktop and app workflows, including:

- ChatGPT Web
- ChatGPT Mac app
- Chrome
- Firefox
- Safari
- Edge
- Brave
- Opera
- macOS
- Windows
- Linux
- shared links
- manual selection
- Ctrl+A / Ctrl+C
- Ctrl+F
- Print / Save as PDF
- Save Page As HTML
- extensions or scripts that depend on page content

The user has also asked OpenAI Support to account for earlier HAR-related diagnostic material submitted in the first case trail before requesting another HAR.

Open questions sent to OpenAI Support:

1. Did OpenAI receive the earlier HAR or HAR-related material in Case 08747965?
2. Where is that material now?
3. Is it attached to Case 08747965, Case 09120830, Case 09371968, or another internal record?
4. Who has had access to it?
5. Has it been deleted, lost, detached, overwritten, or made unavailable?
6. What retention rule applies to it?
7. Why is a new HAR required when Case 08747965 was already summarized as escalated to ChatGPT Web engineering?

A HAR file can contain account, session, request, URL, timing, and other diagnostic data. A screen recording can expose account state, sidebar items, project names, conversation titles, and transcript material. These are not low-risk files.

The user has refused to provide further private HAR files, private affected conversation URLs, or private screen recordings as a routing prerequisite while OpenAI has not accounted for the earlier diagnostic material.

The user has also cancelled ChatGPT Plus, citing the handling of this issue as a major reason.

The core product issue remains unchanged:

ChatGPT presents a conversation as one transcript, while browser-level operations may act on only part of it. This affects search, copy, manual selection, print, PDF, HTML save, shared-link preservation, and extension/export routes that depend on page content.

Expected behavior:

A user-visible conversation should be available as one conversation object for search, copy, manual selection, print, PDF, HTML save, shared-link preservation, and export.

Observed behavior:

Those paths may act on only part of the transcript while the UI presents the conversation as complete.

Suggested internal repro remains simple:

1. Open ChatGPT Web in a signed-in test account.
2. Create marker messages such as START_TEST_123, MIDDLE_TEST_123, and END_TEST_123.
3. Use Ctrl+F before and after scrolling.
4. Use Ctrl+A / Ctrl+C and paste into a plain text editor.
5. Try manual selection.
6. Try Print / Save as PDF.
7. Try Save Page As HTML.
8. Check whether all markers appear in each result.

If OpenAI views transcript virtualization as expected product behavior, users need a full-transcript Archive / Print / Search mode and warnings when browser-level operations do not cover the full conversation.

If OpenAI views this as an unintended regression, it needs ChatGPT Web engineering handling without making private user diagnostic artifacts a gate for routing.


Chrome Ctrl+F misses text in long ChatGPT threads, match count changes with scroll position
Silent partial transcript exposure in long ChatGPT conversations affects search, copy, print, PDF, and HTML save

Browser:
Chrome / Firefox / Edge / Brave / Opera

OS:
Linux / Windows / macOS

Thread length:
short / medium / very long

Tests:
1. Ctrl+F known repeated marker at top, middle, bottom scroll positions.
2. Ctrl+A / Ctrl+C into plain text editor.
3. Print / Save as PDF.
4. Save Page As HTML.
5. Compare first marker, middle marker, final marker.
6. Record whether match counts change after scrolling.

Additional reproduction: Chrome in-page search is also affected.

In the same long ChatGPT thread, Ctrl+F and search for a known repeated marker, for example "Thought for"

Expected:
A stable count of all matches in the full conversation, e.g. 8 or 9.

Observed:
Chrome reports only 3 to 5 matches, and the count changes depending on scroll position.

This suggests the issue is not limited to copy, print, PDF, or Save Page As. Browser-level whole-page functions appear to see only part of the long ChatGPT transcript, likely whichever sections are currently mounted or retained by the page.

Impact:
Users cannot rely on Ctrl+F to audit long chats.
Users cannot reliably verify whether a backup contains all sections.
Search whole page is core archival functionality, not a minor convenience.

Related failures already observed:
Ctrl+A / Ctrl+C can miss sections.
Print / Save as PDF can miss sections.
Save Page As HTML can miss sections.
Ctrl+F can miss matches and vary by scroll position.

Danger:
The page looks like one continuous transcript, but browser operations may silently operate on a partial transcript.

partial_backups =
daily_active_users
* affected_backup_user_rate
* affected_method_rate
* partial_failure_rate
* days

missing_bytes =
partial_backups
* max(0, intended_transcript_bytes - saved_fragment_bytes)

* This should not be dismissed as a niche 1MB monster-chat problem.

Even if only 0.01% of ChatGPT weekly users attempt an affected single-chat backup on a given day, and only 20% of those attempts fail partially, that still implies thousands of silent partial backups per day.

Across months, the plausible scale is hundreds of thousands to millions of misleading local backup artifacts.

The byte count is less important than the trust failure: users may delete, move on, cite, archive, or rely on a backup that silently omitted parts of the conversation.

Potentially millions of partial local backups, with missing content plausibly in the tens of GB to low TB range over months, depending on how many users tried single-chat backup methods during the affected period.

With ChatGPT operating at hundreds of millions of weekly users and billions of messages per day, even a tiny affected-backup-user rate can produce thousands of silent partial backup artifacts per day. Over a multi-month period, this plausibly reaches hundreds of thousands to low millions of partial backups.

Update: a third distinct user has now confirmed reporting the issue to OpenAI Support. This user says they opened multiple tickets and tested Chrome, Edge, Brave, Opera, Firefox, browser print, system print dialog, Save as PDF, XPS, extensions, shared links, copy/paste, and scripts. They report that every route has some failure mode, and describe the issue as a regression being treated as a minor inconvenience rather than a data portability and archival issue.

2026-05-16 update:
A separate Facebook group post has now appeared describing trouble preserving very long ChatGPT conversations. The user reports failures when trying to copy/export/share/paste long chats into Word, reproduced on more than one computer. In follow-up comments pasted by a reader, the user says the issue remains unresolved after account verification and that they have not received a meaningful support response.

This is not yet evidence for the short-thread variant, but it is independent public chatter in the same conversation-preservation/export failure family.

2026-05-19 update:
A separate Facebook user has publicly reported inability to preserve full ChatGPT conversations. Reported paths include copy/paste into Word, shared conversation copy/paste, multiple PCs, multiple browsers, private browsing, Word, Notepad, shared links, logout/login, new browser sessions, and clearing ChatGPT/OpenAI site data and cookies. They state the core issue persisted after site-data reset and that shared conversations still pasted as only a small portion of the expected chat. They list OpenAI Support Case 08816421 and say they have sent repeated escalation messages without a substantive human explanation or fix.

Multiple users have independently reported ChatGPT conversation preservation/export failures to OpenAI Support, including at least two public support case trails.

2026-05-22 update:
OpenAI is reportedly preparing for a possible IPO. That makes this issue more serious, not less.

Users are reporting that ChatGPT conversations may appear available in the UI while copy, search, print, PDF, HTML save, shared-link, app, and extension workflows can expose only part of the transcript.

That is not just a support nuisance. It is data portability, archive integrity, and customer trust.

The problem is not one user, one browser, or one private transcript. Reports now cover Chrome, Firefox, Safari, Edge, Brave, Opera, macOS, Windows, Linux, ChatGPT Mac app, shared links, manual selection, extensions, and ordinary desktop/web workflows.

If OpenAI is moving toward public-market scrutiny, this needs product-owner and engineering handling, not an evidence loop that asks affected users for private recordings and HAR files before routing.

2026-05-27 update:
Another Reddit user reports that OpenAI has not meaningfully responded for over a week after they supplied browser details, confirmed the issue across multiple devices, and tried cache/cookie resets. This adds to the support-process pattern: affected users are providing environment and repro data, but support continues to request private recordings/HAR files or goes silent, while the issue remains active.

2026-05-29 update:
A new r/ChatGPT post by another user frames the transcript preservation issue as part of a wider failure to serve independent high-volume users. The post specifically says copy/paste of conversations became impossible this month, links the existing Reddit bug thread, and argues that slow account export is not a usable substitute for per-chat preservation. It also connects the issue to workspace reliability: users need to preserve questions, answers, pivots, drafts, and development history, not only final outputs.
https://www.reddit.com/r/ChatGPT/comments/1tr7snh/chatgpt_is_completely_neglecting_independent/
