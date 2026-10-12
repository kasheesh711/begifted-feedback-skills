# BeGifted feedback for Claude Code

Use this package to check your own completed classes from the past 72 hours, then add feedback from your notes. Each comment must contain at least 300 characters. This package contains no tutor account, student records, or login data.

## Install

1. Extract this ZIP file.
2. Copy its `begifted-daily-feedback` folder into `~/.claude/skills/`. The final file must be `~/.claude/skills/begifted-daily-feedback/SKILL.md`. If that folder already exists, compare the files before replacing it. Personal skills are available across projects. See [Claude Code skills](https://code.claude.com/docs/en/skills).
3. Open Chrome and sign in to your own BeGifted account at https://learn.begiftededucation.com/get-started.
4. Install or enable the official Claude in Chrome extension. Use an eligible direct Anthropic plan and sign in to Claude Code with `/login`. Start Claude Code with `claude --chrome`. Run `/chrome` to check the connection. Allow access to the BeGifted site when requested. See [browser setup](https://code.claude.com/docs/en/chrome).

If browser tools are unavailable, the skill can prepare drafts from your notes, but it cannot check or submit live website feedback. Do not use a draft as proof of a saved comment.

## First check

Replace the example name with your full BeGifted tutor name:

```text
/begifted-daily-feedback Check completed classes from the past 72 hours for tutor [your full tutor name]. Use Bangkok time. Give me a short list of missing comments. Do not enter or submit feedback.
```

If you use separate online and in-person profiles, name the profiles you want checked. Claude must confirm the host of each class. If your account does not provide the required views, the check must report its limits.

## Add comments

Reply in the same chat after the check:

```text
Write and submit feedback for the listed classes using these notes. Each comment must have at least 300 characters. You may make reasonable deductions from my notes, but do not invent scores or homework. Check each saved comment after reopening its class.

Student, subject, class date and time:
Attendance:
Topics covered:
How the student did:
Areas for practice:
Homework and deadline, if assigned:
```

Include separate notes for each class. If two classes should have the same feedback, say which ones. For drafts only, replace “Write and submit” with “Prepare drafts only”.

## Optional daily check

First complete one live check. Then choose a local scheduler that has access to your signed-in browser. Use this task prompt, with your own name:

```text
Use /begifted-daily-feedback to check completed classes for tutor [your full tutor name] from the previous 72 hours at the actual run time. Report missing comments with student, subject, date, and time in Asia/Bangkok. Give the result each day, even if unchanged. Report an access failure as an incomplete check. Do not write or submit feedback or change attendance. Wait for my class notes.
```

Claude Code Desktop supports local scheduled tasks; confirm that the task can access the browser tools before enabling daily use. Run its “Run now” check first. The machine and app must be available. A CLI session schedule runs while Claude Code is running and expires after seven days. Scheduling uses local time, so confirm that 21:00 means Bangkok time or convert it. See [scheduling options](https://code.claude.com/docs/en/scheduled-tasks) and [Desktop tasks](https://code.claude.com/docs/en/desktop-scheduled-tasks).

The ZIP does not create a schedule. Claude Code browser use and other tutors' account permissions have not been tested with this package.
