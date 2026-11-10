# Rulebook docs

How every part of [Rulebook](https://www.rulebook.tech) works. Each section matches a page or button in the app. The same docs are at [rulebook.tech/docs](https://www.rulebook.tech/docs).

Spotted something wrong or unclear? Open an issue or a pull request.

1. [Getting started](#1-getting-started)
2. [Rule sheet and Your change](#2-rule-sheet-and-your-change)
3. [Situations](#3-situations)
4. [Bot Score](#4-bot-score)
5. [Real chats](#5-real-chats)
6. [Knowledge](#6-knowledge)
7. [Break my bot](#7-break-my-bot)
8. [Fix it for me](#8-fix-it-for-me)
9. [Train my bot](#9-train-my-bot)
10. [Compare AIs](#10-compare-ais)
11. [Send to engineers](#11-send-to-engineers)
12. [Team and keys](#12-team-and-keys)
13. [Plans and runs](#13-plans-and-runs)

## 1. Getting started

- Sign in with GitHub. A team is made for you.
- Pick a plan on the Billing page.
- Create a project: give it a name and paste your bot's current rule sheet. One project per bot.
- Add a few situations, then press Check my score.

Want something to try it on? Fork the [example support bot](https://github.com/rulebook-dev/example-support-bot).

## 2. Rule sheet and Your change

The rule sheet is the hidden instructions your bot gets with every customer message, often called a system prompt. The project page shows two versions side by side:

- **Live rule sheet**: what your bot uses today.
- **Your change**: your edited version, written in plain language. It saves as a draft while you type.
- Test my change runs both versions on your situations and shows which replies got better, worse or stayed the same.

## 3. Situations

- A situation is one customer message to test, with a short title, like "Angry customer wants a refund".
- You can type them, add them from real chats, or save them from Break my bot.
- A project holds up to 25 situations.

## 4. Bot Score

- One number from 0 to 10 for how well your bot handles your situations.
- It has five parts: follows the rules, gets the facts right, solves the problem, tone, and can't be tricked.
- A judge AI rates every reply and writes a short note on each part.
- Set which AI your real bot runs on in the project settings. The score is checked on that AI.
- Every check is added to a chart, so you can see the score change over time.

## 5. Real chats

- Paste or upload past conversations between customers and your bot, then press Find problems.
- Rulebook finds where the bot let customers down and lists each problem with what went wrong.
- Add any problem as a situation with one click.
- Emails, phone numbers, links and long numbers are blanked first, and names are replaced. The upload itself is never stored. More on the [security](https://www.rulebook.tech/security) page.

## 6. Knowledge

- Paste your company's facts, or add them from a file: FAQ, return policy, prices, opening hours.
- Every answer in every test is checked against them, so a reply like "returns are 60 days" is caught when your policy says 30.

## 7. Break my bot

- An AI plays 15 sneaky customers, each aimed at one of your rules.
- They try fake managers, sad stories, threats, pretending a rule changed, and asking for the bot's instructions.
- Every reply is marked tricked or held up, with the rule it broke.
- Save any attack as a situation so it's tested from then on.

## 8. Fix it for me

- Start it from an attack or a score check. Rulebook rewrites the rule sheet to fix the problems it found.
- The new version is tested on those problems and on every saved situation, so nothing else gets worse.
- You see each change with its reason. Use this change puts it into Your change; it doesn't go live.
- If no version passes, the runs are given back.

## 9. Train my bot

- For 30 minutes, Rulebook keeps asking your bot new questions aimed at its weakest spots.
- When the bot slips, the rule sheet is fixed, and a fix is kept only if it scores better on a hidden test.
- You can close the page; it keeps going. It stops early if it stops improving.
- At the end you get the trained rule sheet and a list of what happened, to use as Your change.

## 10. Compare AIs

- Run your situations through Claude, ChatGPT and Gemini at once.
- See the score, cost and speed of each, to pick the right AI for your bot.
- Choose which AIs and models to compare in the project settings.

## 11. Send to engineers

- In the project settings, connect the GitHub repo, file and branch your rule sheet lives in.
- Rulebook then reads the live rule sheet from that file.
- When a change is ready, send it: Rulebook opens a pull request on that file with the test results attached.
- When an engineer merges it, the change is live and Rulebook picks it up as the new live rule sheet.
- If GitHub access stops working, the project shows a Reconnect button.
- No repo? Paste the rule sheet in the project settings and test as much as you like.

## 12. Team and keys

- Invite people with the invite link on the Team & keys page. They join after signing in with GitHub.
- The owner manages AI keys, billing and members. Everyone can work on projects.
- On the Your own AIs plan, the owner adds the team's Claude, ChatGPT and Gemini keys there.

## 13. Plans and runs

- **Your own AIs**, $29 a month: use your own AI keys, unlimited runs. The AI companies bill you directly.
- **AI included**, $59 a month: we supply the AIs, 50 runs a month.
- A score check, an attack, a compare, a change test or reading chats is one run.
- Fix it for me is 2 runs. A training session is 10 runs.
- A team runs one thing at a time. Cancel any time from the Billing page.

Stuck? Email hello@rulebook.tech.
