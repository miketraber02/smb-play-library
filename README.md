# SMB Play Library

A small set of plays for Netlify's Tech Touch book, with one job: **find out which first messages land, and keep improving them.**

Each play is a **trigger** (what you see in the data), **who gets the first message**, **one versioned first message** (01-A),
a **hand-off rule**, and **what success looks like**. Every send is logged, and a weekly review keeps the winner and writes a version B to beat it.

**Landing** = took the action within 14 days (headline). Replied = early read.
Built with the 5-step algorithm: question the requirements, delete, simplify, speed up, automate last.

Started by Mike in Nov 2026, because there was no SMB playbook yet (said by Matt Gargano in interviews).

## Rules
- Practice data only. Every account in this repo is made up. Real customer work happens in Netlify's own tools.
- Every fact gets a tag: [Said] someone told us, [Public] netlify.com or docs, [Confirm] still a question.
- Pricing changes. Re-check any number before you use it with a customer.
- Messages follow one voice: direct, specific, proof before claim, one idea per sentence, no em dashes.

## How to add a play
1. Open `index.html`. Find a block that starts with `<!-- PLAY 0X -->`.
2. Copy the whole `<div class="card">` block and paste it under the last play.
3. Change the number, fill in every label, and write one first message labeled with a version ID (05-A).
4. Add the version to the dropdown in the Log a send form and a row to the weekly review table.
5. Open a pull request. Check the Deploy Preview link. Merge when it looks right.

## How to test a new version
1. Under about 10 sends, don't call a winner. Read the notes.
2. Write version B (01-B) and change one thing only, so you know what made the difference.
3. Add it to the form dropdown. Keep the old version until the new one wins.

## Reference: the Tuesday loop
1. Open the account list (in Netlify's own tools). Look for accounts that match a play's trigger.
2. Pick the play, then the person. The play says who gets the first message.
3. Send one message. Hand off what isn't yours: bugs and odd traffic to Support, plan changes past Pro to Sales [Confirm the exact rules].
4. After 7 days, log the send and its outcome.

Why it exists: Tech Touch accounts get a welcome email, then mostly silence until about 90 days before renewal [Said, Matt].
Measured on retention against an 85% target [Said]. Pipeline is an unofficial target [Said].

## Reference: who to talk to
| Role | Who they usually are | What they care about | What you give them |
|---|---|---|---|
| User | The developer, or whoever builds with AI and deploys | Shipping without things breaking | A fix, a setting, a how-to |
| Champion | Whoever brought Netlify in or defends it | Looking right for picking Netlify | Proof it works, early warning |
| Renewal signer | Owner, founder, finance, IT. May never log in. | Cost, risk, one clear decision | A choice with a price. Two options, max. |

Only a Team Owner can turn auto recharge on or off [Public, docs, Nov 2026].

## Files
- `index.html` how it learns, the plays, the send log form, and the weekly review
- `logged.html` the page you land on after logging an outcome

## Version log
- v1 (Nov 19, 2026): Plays 01 Credit cliff, 02 Gone quiet, 03 Team outgrew its login.
- v1.1 (Nov 21, 2026): Play 04 Stuck at first deploy, from Mike's own confusion on the build settings page.
- v1.2 (Nov 21, 2026): First change made by Mike.
- v2.0 (Nov 24, 2026): One job: track which first messages land. One versioned first message per play, a 5-field send log, a weekly review. Tuesday loop and role table moved here. The other role templates from v1.1 were deleted on purpose; they're in git history (commit `4d64e01`, the last v1 version) if any earn their way back.
- v2.1 (Nov 24, 2026): Log each send once, at 7 days. Count results from the Forms list; no CSV download.
