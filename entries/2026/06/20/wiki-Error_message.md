---
source: sources/wiki-Error_message.md
source_url: https://en.wikipedia.org/wiki/Error_message
---

## Error Messages in Computing

This page covers the concept of error messages — short text messages that inform users about problematic situations in software. It addresses how error messages are presented, what content they should contain, notable historical examples, and the modern trend of "fail pets" used by web services. Error message design is positioned as a key concern in usability and human-computer interaction.

## Key Concepts

- An **error message** is a short text message describing a failed operation, often directing the user toward corrective action.
- Error messages are distinct from other error information like core dumps or stack traces, which provide diagnostic data but are not "messages" per se.
- Error information can be classified as: **error**, **warning** (potential problem), or **informational** (no problem).
- Abstract error representations (indicator lights, numeric displays) may require consulting documentation to interpret.
- Error messages can be delivered via GUI dialog boxes, CLI standard streams, or log files.
- **Security consideration**: error messages should never expose information exploitable by attackers (e.g., distinguishing "invalid user" vs. "invalid password" leaks account existence).
- Three main design factors: **technical limitations**, **amount of information**, and **required user input**.

## Commands and Syntax

No specific commands per se, but notable error message strings include:

- `?` — the `ed` text editor's response to nearly all errors
- `Abort, Retry, Fail?` — MS-DOS error prompt
- `Bad command or file name` — MS-DOS
- `PC LOAD LETTER` — HP LaserJet printers requesting Letter-size paper
- `SYNTAX ERROR` — older computing environments for unrecognized instructions
- `Error 1603` — Windows installation failure
- `lp0 on fire` — Unix printer warning
- `ENOTTY` / `Not a typewriter` — Unix error with a historically misleading name
- HTTP status codes: **404** (resource not found), **500** (server error)

## Relationships

- **Usability / HCI**: Error message design is a sub-discipline of usability engineering and human-computer interaction.
- **Exception handling**: Error messages are the user-facing output of programmatic exception handling.
- **Alert dialog boxes**: Modal error dialogs are one presentation mechanism.
- **HTTP status codes**: Web error messages map to standardized HTTP codes (404, 500, etc.).
- **Kernel panics / BSODs**: Critical system-level errors have their own specialized error displays (Blue Screen of Death on Windows, Guru Meditation on Amiga, kernel panic on Unix/Linux/macOS).
- **Brand identity**: "Fail pets" connect error messages to marketing and brand awareness strategy.

## Exam-Relevant Points

- Error messages should **never leak security-sensitive information** (e.g., confirming whether a username exists).
- The three factors governing error message design: **technical limitations**, **information volume**, and **user input requirements**.
- **Presentation methods**: modal dialog boxes (block interaction), notification icons (non-modal), and status bars.
- Common error conditions to recognize: Access denied, Device not ready, File not found, Low Disk Space, Out of memory, HTTP 404.
- **Blue Screen of Death (BSoD)** is the Windows equivalent of a **kernel panic** on Unix/Linux/macOS.
- The term **"Fail Pet"** was coined by Mozilla engineer Fred Wenzel; Twitter's **Fail Whale** is the most famous example.
- In POSIX, a success status code can be confusingly reported as an error — a sloppy error-handling antipattern.
- `ed`'s single `?` response is a canonical example of an unhelpful error message.
