# SMB Play Library

A small, growing set of plays for Netlify's Tech Touch book. Each play is:
a **trigger** (what you see in the data), **who gets the first message**, a **template for each role**
(user, champion, renewal signer), a **hand-off rule**, and **what success looks like**.
Every send gets logged so the library learns which messages work.

Started by Mike in Nov 2026, because there was no SMB playbook yet (said by Matt Gargano in interviews).

## Rules
- Practice data only. Every account in this repo is made up. Real customer work happens in Netlify's own tools.
- Every fact gets a tag: [Said] someone told us, [Public] netlify.com or docs, [Confirm] still a question.
- Pricing changes. Re-check any number before you use it with a customer.
- Messages follow one voice: direct, specific, proof before claim, one idea per sentence, no em dashes.

## How to add a play
1. Open `index.html`. Find a block that starts with `<!-- PLAY 0X -->`.
2. Copy the whole `<div class="card">` block and paste it under the last play.
3. Change the number, fill in every label, write three templates.
4. Add the play to the dropdown in the Outcome log form.
5. Open a pull request. Check the Deploy Preview link. Merge when it looks right.

## Files
- `index.html` the library, the Tuesday loop, the role table, and the outcome log form
- `logged.html` the page you land on after logging an outcome

## Version log
- v1 (Nov 19, 2026): Plays 01 Credit cliff, 02 Gone quiet, 03 Team outgrew its login.
- v1.1 (Nov 21, 2026): Play 04 Stuck at first deploy, from Mike's own confusion on the build settings page.
- v1.2 (Nov 21, 2026): First change made by Mike.
