# BeGifted feedback for Codex

Use this package to check your own completed classes from the past 72 hours, then add feedback from your notes. Each comment must contain at least 300 characters. This package contains no tutor account, student records, or login data.

## Install

1. Extract this ZIP file.
2. Copy its `begifted-daily-feedback` folder into your Codex skills folder. This is normally `~/.codex/skills/`, or `$CODEX_HOME/skills/` if you use a custom Codex home. The final file must be `skills/begifted-daily-feedback/SKILL.md` inside that folder. If the skill already exists, compare the files before replacing it.
3. Start a new Codex chat so that it can discover the skill.
4. Sign in to your own BeGifted account at https://learn.begiftededucation.com/get-started in a browser Codex can control. Use a Codex session with browser or Computer Use tools. The skill file alone does not provide browser access. The tested Mac setup used Computer Use with Safari. Ask Codex to find the required browser-control plugin if these tools are unavailable. Recording a new demonstration is not required.

If browser tools are unavailable, Codex can prepare drafts from your notes, but it cannot check or submit live website feedback. Do not use a draft as proof of a saved comment.

## First check

Replace the example name with your full BeGifted tutor name:

```text
Use $begifted-daily-feedback. Check completed classes from the past 72 hours for tutor [your full tutor name]. Use Bangkok time. Give me a short list of missing comments. Do not enter or submit feedback.
```

If you use separate online and in-person profiles, name the profiles you want checked. Codex must confirm the host of each class. If your account does not provide the required views, the check must report its limits.

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

First complete one live check. Then ask Codex in the same chat:

```text
Create a daily check at 21:00 Asia/Bangkok. Use $begifted-daily-feedback to check completed classes for tutor [your full tutor name] from the previous 72 hours at the actual run time. Report missing comments with student, subject, date, and time in Asia/Bangkok. Give the result each day, even if unchanged. Report an access failure as an incomplete check. Do not write or submit feedback or change attendance. Wait for my class notes.
```

Confirm that Codex reports a saved, active schedule. Check the first scheduled result. Local browser checks need the computer, Codex, and the signed-in browser to be available. If your Codex setup has no scheduler, run the skill manually.

The ZIP does not create a schedule. The original workflow was tested in one Codex/Safari account; this general version and other tutors' account permissions have not been tested live.
