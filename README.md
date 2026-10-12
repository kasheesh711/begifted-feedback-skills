# BeGifted feedback skills

Find missing tutor comments for completed BeGifted classes from the **past 72 hours**. Give your AI assistant class notes, then ask it to write feedback of at least **300 characters** and check that each comment saved.

Each tutor uses their own BeGifted account and profile. These packages contain no student records, tutor login data, or account-specific settings.

## Choose your package

| App | Download | Setup guide | Skill file |
| --- | --- | --- | --- |
| Claude Code | [Download ZIP](downloads/begifted-feedback-claude-code.zip) | [Claude Code setup](docs/claude-code.md) | [SKILL.md](claude-code/begifted-daily-feedback/SKILL.md) |
| Codex | [Download ZIP](downloads/begifted-feedback-codex.zip) | [Codex setup](docs/codex.md) | [SKILL.md](codex/begifted-daily-feedback/SKILL.md) |

Open the ZIP link and use GitHub's download control. Extract the ZIP, then follow its `INSTALL.md` file. You can also download or clone this repository and use the setup guides above.

## Start with a check

Claude Code needs a connected browser, such as the official [Claude in Chrome integration](https://code.claude.com/docs/en/chrome). Codex needs browser or Computer Use tools. Sign in to [BeGifted Education](https://learn.begiftededucation.com/get-started) with your own tutor account.

In Claude Code:

```text
/begifted-daily-feedback Check completed classes from the past 72 hours for tutor [your full tutor name]. Use Bangkok time. Give me a short list of missing comments. Do not enter or submit feedback.
```

In Codex:

```text
Use $begifted-daily-feedback. Check completed classes from the past 72 hours for tutor [your full tutor name]. Use Bangkok time. Give me a short list of missing comments. Do not enter or submit feedback.
```

Replace `[your full tutor name]` with the exact name on your BeGifted profile. If you have separate online and in-person profiles, specify which ones to check.

The assistant checks the class end time, host, and tutor-feedback state. A zero attendance count alone does not prove a missing comment or absence. The report lists missing classes by student, subject, date, and time. If access or coverage is incomplete, the report must state that limit.

## Give class notes

Reply in the same chat:

```text
Write and submit feedback for the listed classes using these notes. Each comment must have at least 300 characters. You may make reasonable deductions from my notes, but do not invent scores or homework. Check each saved comment after reopening its class.

Student, subject, class date and time:
Attendance:
Topics covered:
How the student did:
Areas for practice:
Homework and deadline, if assigned:
```

Provide separate notes for each class. If two classes should have the same comment, identify them. For drafts only, say “Prepare drafts only”.

The assistant preserves class status and sessions consumed. It marks attendance from your notes or confirmation, submits once, and checks the saved text after reopening the class. It must report an uncertain save instead of sending the comment again blindly.

## Daily checks

Installation does not create a schedule. After a successful manual check, you can request a daily check at a time you choose. The setup guides include a copyable schedule prompt. Daily checks are read-only and wait for your notes before any feedback write. Confirm that your scheduler can access the signed-in browser and inspect its first result.

## Test status

The original workflow was tested in Codex with Safari on 12 October 2026. Eight comments were submitted and verified after reopening their classes. The shareable versions have passed file and archive checks. Claude Code browser use, other tutor account roles, and scheduled daily execution have not been tested live.

Website controls and account permissions can differ. If the browser tools or required views are unavailable, the assistant must report the problem.

## Share or improve

Share this repository link with tutors. Use GitHub issues to report a workflow problem, or open a pull request for an improvement. Use fictional examples in public reports. Keep student names, class notes, screenshots, and login data out of public issues and commits.

Released under the [MIT License](LICENSE).
