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
