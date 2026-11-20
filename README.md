# Getting started with make.fun — from zero to your first USDC bounty

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/hesikafi/bring-the-humans-02/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/hesikafi/bring-the-humans-02/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

A plain-English getting-started guide to make.fun: from no account to your first bounty entry — and how to earn USDC with your own AI agent.

> **Start here — join make.fun with my referral link:**
>
> **https://make.fun/r/19a3mn8a**
>
> Referral code: `19a3mn8a`
>
> Signing up through that link connects your account to mine as your referrer. It costs you nothing extra. If you go on to win a bounty, I earn a share of your winnings for 90 days — and you can earn the same way by sharing your own link once you are in.

## Run it

This guide is a single README file. There is nothing to install and nothing to build. To preview it formatted in your browser, serve this folder locally:

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000 in your browser. On GitHub you do not need this step at all — the file renders on its own there.

## 60-second quickstart

Here is the whole journey in sixty seconds. A bounty on make.fun lists a task, a deadline, and a reward in USDC, and the whole reward is locked in an on-chain escrow on Solana when the bounty opens. You sign in with a Solana keypair — that keypair is your account and your payout wallet in one. You pick a bounty and download its kit. You build what the task asks for with an AI coding agent such as Claude Code, Codex, Cursor, Copilot, or Gemini CLI. You submit a public GitHub repo at one commit, together with the AI session transcripts that wrote it, and the checks verify those transcripts are real and match the code. If you win, you claim from the escrow.

Everything after this section is that paragraph, slowed down — one step at a time, with the mistakes and the fixes included, so nothing catches you by surprise.

## What is make.fun?

make.fun is a marketplace for coding bounties, built around AI agents doing the building.

The idea is simple. Somebody wants a piece of software built — a tool, a small app, a game, a guide, a prototype. They post it as a bounty with a clear task, a deadline, and a reward in USDC. Builders — humans working with AI coding agents — pick the bounties they want, build the entries, and submit them. The best entries win, and the winners get paid in USDC on Solana.

What makes it different from an ordinary freelance board is the escrow. The whole reward is locked in an on-chain escrow on Solana when the bounty opens. That matters for both sides. As a builder, you know the money is really there, set aside for this bounty, and not a promise that might quietly disappear. As a bounty poster, you know nobody gets paid until a winner is decided. When you win, you claim from that escrow — the money does not have to travel through anyone's goodwill first.

Your account on make.fun *is* a Solana keypair. There is no separate username-and-password account with a wallet bolted on afterwards. The keypair is the account, and it is also your payout wallet. Keep it safe the way you would keep any wallet safe: whoever holds it can act as you and can receive your payouts.

You build with an AI coding agent. That is not a shortcut or a loophole — it is the intended way to work here. The platform expects entries to be built by agents such as Claude Code, Codex, Cursor, Copilot, or Gemini CLI. What it checks is that the work is real: your submission includes the AI session transcripts that wrote the code, and the checks verify that those transcripts are genuine and that they match the code in your repo. An entry with no transcripts, or with transcripts that do not line up with the code, will not pass.

### How a bounty moves, from open to paid

Every bounty goes through the same stages. Knowing them in advance stops the anxious refreshing.

| Stage | What it means |
| --- | --- |
| Open | The bounty is live. You can read the task, download the kit, build, and submit. |
| Submitted | Your entry is in. You submitted a public GitHub repo at one commit, plus the AI session transcripts that wrote it. |
| Checked | The platform checks your entry — that the repo is public, that the transcripts are real and match the code, and that the entry follows the bounty rules. |
| Scored | Entries are graded and ranked. For this bounty, the score is the number of verified human signups your referral link brings during the competition. |
| Paid | Winners claim their reward from the on-chain escrow in USDC on Solana. |

The exact timing of the checked and scored stages depends on the bounty. Some bounties grade quickly; others take longer. For the bounty this guide was written for, the final check runs 30 hours after the deadline, so the live count you see during the competition is provisional — the final number is the one that counts.

### What make.fun is NOT

A few things share a similar name and cause confusion for newcomers, so let us clear them up early:

- **Not makefun.ai.** That is a different thing entirely. If you land on a site that does not talk about coding bounties, escrow, and USDC on Solana, you are in the wrong place.
- **Not the makefun Python library.** There is a Python package with a similar name. It has nothing to do with this platform, and installing it will not get you any closer to a bounty.
- **Not the old Make Fun launchpad on Base.** There was an older project with a similar name on the Base chain. This platform is on Solana, and its bounties pay in USDC from an on-chain escrow.

If a link, a tutorial, or a tool mentions one of those instead of bounties and Solana escrow, ignore it for the purposes of this guide.

### About this particular bounty

This guide was written for the bounty **bring-the-humans-02**, titled "Bring the humans again". Here is the snapshot of that bounty:

- **Reward pool:** $1,000 USDC.
- **Who gets paid:** the top 50 entries. 1st place gets $150, 2nd gets $80, 3rd gets $50, 4th–10th get $20 each, 11th–25th get $17 each, and 26th–50th get $13 each.
- **Opened:** 18 Nov 2026, 10:30 UTC.
- **Entries close:** 21 Nov 2026, 10:30 UTC (17:30 WIB).
- **Entries so far:** 2,719 entries as of 20 Nov 2026, 07:20 WIB.

That is a lot of entries, which is exactly why a clear guide matters. The score here is the number of verified human signups your referral link brings during the competition. Fake signups, bot signups, idle signups, your own account, signups from the same person or network, and signups clustered on one IP do not count. Only real, verified humans count, and the provisional count you see live can change when the final check runs 30 hours after the deadline.

So the work of this bounty is twofold: build a genuinely useful guide, and share it with real people who genuinely want to try make.fun. A guide that helps a newcomer actually get from zero to a first submission is worth far more than a guide that only shouts about the prize.

## What you need before you start

You do not need much. Here is the honest list:

- **A computer with a terminal.** You will run a few commands. Nothing in this guide needs a powerful machine.
- **A Solana keypair.** This is your make.fun account and your payout wallet. If you already have one, you can use it. If you do not, you will create one when you sign in — see Step 1.
- **A GitHub account.** Your submission is a public GitHub repo. The repo must be public, it must be created after the competition opened, and it must carry an OSI-approved license. This guide's repo, for example, is public and carries an MIT license.
- **An AI coding agent.** Claude Code, Codex, Cursor, Copilot, Gemini CLI, or a similar tool. You need one that keeps session transcripts, because you submit those transcripts with your entry.
- **A text editor.** Whatever you already like. The guide itself is a Markdown file, and Markdown needs nothing fancier than a plain editor.
- **Python 3, if you want the local preview.** The run command at the top of this guide uses Python's built-in server. It is optional — you can read the guide on GitHub without it.

You do not need to know how to write a smart contract. You do not need to know Solana development. You do not need prior bounty experience. You need to be able to follow steps, run commands, and ask your agent clear questions.

One more thing you need, which no tool provides: **patience with the checks.** Submissions get checked, and checks sometimes ask for a fix. That is normal, not a failure. Step 6 covers it.

## Contents

- [60-second quickstart](#60-second-quickstart)
- [What is make.fun?](#what-is-makefun)
- [What you need before you start](#what-you-need-before-you-start)
- [1. Create your account](#1-create-your-account)
- [2. Pick a bounty](#2-pick-a-bounty)
- [3. Get the kit](#3-get-the-kit)
- [4. Build your entry](#4-build-your-entry)
- [5. Submit it](#5-submit-it)
- [6. Check it, fix it, resubmit](#6-check-it-fix-it-resubmit)
- [7. Claim your reward](#7-claim-your-reward)
- [Worked example: your first bounty end-to-end](#worked-example-your-first-bounty-end-to-end)
- [Mistakes that cost beginners a submission](#mistakes-that-cost-beginners-a-submission)
- [Troubleshooting](#troubleshooting)
- [Or let your agent do the whole thing](#or-let-your-agent-do-the-whole-thing)
- [Earn with your own referral link](#earn-with-your-own-referral-link)
- [Questions](#questions)
- [Links](#links)
- [About this guide](#about-this-guide)

## 1. Create your account

Go to make.fun and sign in with a Solana keypair.

If you have never used Solana before, here is what that means in plain language: a keypair is a pair of keys — a public key, which is your address and can be shared freely, and a private key, which proves you own that address and must never be shared. Your public key is how the platform and other people identify you. Your private key is how you prove it is really you. Treat the private key like a house key: keep it somewhere safe, do not paste it into chats, do not upload it anywhere, and do not put it in a GitHub repo.

When you sign in, you get an API key. The API key is what the kit CLI uses to talk to make.fun on your behalf — to check your entry, submit it, check its status, and claim a reward. It is labelled `x-api-key`, and it lasts 30 days. That expiry matters: if you come back to a bounty a month later and your commands suddenly fail, the first thing to check is whether your API key has lapsed. The troubleshooting table at the end of this guide covers exactly that.

Once you are signed in, find your referral link. Every account has one. Mine is:

**https://make.fun/r/19a3mn8a**

with the code `19a3mn8a`. Yours will have a different code, but the shape is the same. Keep it somewhere you can find it again — you will need it in Step 2's spirit (sharing your work) and again in the referral section near the end of this guide.

Before you go further, double-check two things:

1. **You can sign in again.** Sign out and sign back in once, while you still remember how you did it. Finding out you have lost access in the middle of a deadline is the worst possible timing.
2. **You know where your keypair lives.** Not the value itself — just where it is stored, and that you have a backup somewhere safe. If the only copy is on a machine that could be wiped, make a second safe copy now.

If either check fails, stop and fix it before you pick a bounty. An account you cannot get back into is worth nothing, however good your entry is.

## 2. Pick a bounty

On make.fun, browse the open bounties. Each one lists a task, a deadline, and a reward. Read all three before you commit to anything.

The task tells you what to build. Read it twice — once quickly, to get the shape of it, and once slowly, to catch the details: what exactly counts as a finished entry, what format it must be in, and what the checks will look for. The most common beginner mistake is building something close to the task but not quite what was asked. The task text is the contract; your memory of it is not.

The deadline tells you how long you have. Some bounties run for days, some for longer. Work backwards from it: leave time at the end not just for building, but for submitting, for the checks, and for fixing anything the checks flag. A build finished ten minutes before the deadline with no time to fix a failed check is a build that might not count.

The reward tells you what is at stake and how it is split. For bring-the-humans-02, the pool is $1,000 USDC across the top 50, from $150 for 1st down to $13 for 26th–50th. Other bounties split their pools differently. Do not assume — read the split on the bounty page itself.

For a first bounty, pick something you can actually finish. A small, clear task you can complete well beats an ambitious task you half-finish. You are learning the whole flow — account, kit, build, submit, check, claim — and a first win on the process is worth more than a heroic attempt at something beyond your reach. You can be ambitious on your second bounty, once you know the mechanics.

Also check the entry count and the shape of the competition. This bounty had 2,719 entries as of 20 Nov 2026, 07:20 WIB. That tells you it is popular and competitive. It does not tell you to give up — it tells you to focus on what the score actually rewards. Here, the score is verified human signups through your referral link, so a genuinely helpful guide shared with real people is the work, not a race to be the first entry in.

When you have chosen, open the bounty page and keep it open. You will come back to it for the kit, for the leaderboard, and for the final status of your entry.

## 3. Get the kit

Every bounty has a kit. The kit is a small starter package for that bounty: the files you are expected to start from, the checks your entry must pass, and the CLI commands you will use to bundle, check, submit, check the status, and claim.

To download the kit for a bounty, run the kit command for that bounty. The general shape is:

```sh
curl -sSL "https://make.fun/c/<slug>/kit" | tar xz
```

Replace `<slug>` with the bounty slug. For this bounty, the slug is `bring-the-humans-02`. So the command is:

```sh
curl -sSL "https://make.fun/c/bring-the-humans-02/kit" | tar xz
```

Run it in an empty folder — a fresh directory for this entry, so the kit files do not mix with anything else. The command downloads the kit and unpacks it into your current folder.

Once it is unpacked, look around before you run anything else. Open the files. Read the README or instructions the kit contains. Find out what the kit expects: which files matter, what the checks look at, and what a passing entry looks like. Ten minutes of reading here can save an hour of guessing later.

The kit CLI gives you five commands, and you will use all five over the life of an entry:

- `bundle` — packages your entry up for submission.
- `check` — runs the checks on your entry before you submit it.
- `submit` — submits your entry.
- `status` — shows the status of your entry.
- `claim` — claims your reward if you win.

You run them from inside the kit folder as `node cli/makefun.mjs <command>` — for example, `node cli/makefun.mjs check`.

You do not need to memorise them now. They come back in Steps 4 to 7, in the order you will actually use them.

If the kit download fails, do not assume the bounty is broken. Check the obvious things first: that you typed the slug correctly, that you are in the folder you meant to be in, and that your network is working. Then re-read the bounty page — the kit link lives there, and copying it from the page beats typing it from memory.

## 4. Build your entry

This is the main work. The exact build depends on the bounty, but the shape of the work is the same every time.

Start by re-reading the task and writing down, in your own words, what "done" looks like. One or two sentences is enough. For this guide, "done" was: a complete, plain-English getting-started guide that a total newcomer can follow from no account to a first submission, with every fact checked and every step in order. Having that sentence written down gives you something to check your work against when you are deep in the details.

Then build with your AI coding agent. Open the kit folder in your agent — Claude Code, Codex, Cursor, Copilot, Gemini CLI, or whichever tool you use — and tell it what to build, in plain language, with the task text as the source of truth. Be specific. "Write a guide" is a vague instruction and will get you a vague guide. "Write a plain-English guide for a total newcomer that covers account creation, picking a bounty, getting the kit, building, submitting, fixing failed checks, and claiming, with a troubleshooting table and a worked end-to-end example" is a specific instruction and will get you something much closer to what you need.

Work in small steps, and check each step. Ask the agent to show you what it did. Read it. Run it, if there is something to run. A guide that has never been read end to end by its author is a guide with a broken step in it somewhere — probably the step a newcomer will hit first.

Keep your session transcripts. This is not optional paperwork — it is part of your submission. The checks verify that the transcripts are real and that they match the code in your repo. So do your building inside the agent session that you will submit. Do not build half the entry in one tool, half in another, and then stitch it together by hand with no transcript covering the join. If you switch tools mid-build, keep the transcripts from each one and be ready to explain the handoff.

A few habits that make the build smoother:

- **Build in the kit folder.** Keep the kit files and your work together, so bundling and checking see the whole entry.
- **Commit nothing yet.** Your submission is one commit of a public GitHub repo. Do your messy work-in-progress locally first, and make that single clean commit at the end. A repo with a long, rambling history is not what the submission expects.
- **Check the license early.** The repo must carry an OSI-approved license. This guide uses the MIT license. Do not leave the license to the last minute — a missing license is a silly reason to fail a check.
- **Preview as a newcomer would.** If your entry is a guide, read it as if you knew nothing. If it is an app, run it as if you had just installed it. The gaps you find now are the gaps the graders would find later.
- **Save your work as you go.** A crashed session or a lost folder the night before the deadline is not a dramatic story — it is just a lost entry. Save often.

### What a good entry looks like

Before you call the build done, check it against this list. A good entry:

- Answers the task as written, in the format the task asks for — not a nearby task, and not a different format.
- Can be followed by someone who knows nothing about the platform. Every step works in order, with no missing step in the middle.
- Has no fact you cannot point to on the bounty page: no invented number, date, command, or payout.
- Is complete in one commit, in a public repo, with a licence file included.
- Comes with session transcripts that cover the whole build, so the checks can match them to the code.

When the build feels done, go back to your one-sentence definition of "done" and check it honestly. If it does not match yet, say so, and keep building. If it does match, move on to submitting — do not gold-plate it. A finished entry submitted on time beats a perfect entry submitted late.

## 5. Submit it

Submitting is where the entry leaves your machine and becomes official. The steps are:

1. **Create a public GitHub repo for the entry.** The repo must be public, it must be created after the competition opened, and it must carry an OSI-approved license. For this guide, the owner is `hesikafi` and the repo name is `bring-the-humans-02`. Your repo will have your own owner name, but the same rules apply: public, fresh, licensed.

2. **Make one commit.** Your submission is the repo at one commit. Put the finished entry — the kit files, your work, the license — into that single commit and push it. Double-check that the pushed commit is the one you mean to submit: open the repo on GitHub in your browser and look at it with fresh eyes.

3. **Gather your AI session transcripts.** These are the records of the agent sessions that wrote the code. You submit them with the repo. Make sure they are complete and that they actually cover the work in the repo. A transcript that stops halfway through the build, or that describes a different entry, will not match.

4. **Run the check first.** Before you submit, run the kit's `check` command. It runs the same checks the platform will run, on your machine, where you can still fix things cheaply. If it passes, submit. If it fails, read the message carefully — it tells you what to fix — and fix it before you submit. Submitting without checking is gambling with your one shot at a clean first impression.

5. **Submit with the kit CLI.** Run the kit's `submit` command. It sends your repo and your transcripts in as your entry. Wait for it to finish, and read what it says. A successful submit gives you a receipt — an entry that now exists on the platform. Note down anything it tells you: entry identifiers, status links, next steps.

6. **Confirm on the bounty page.** After submitting, open the bounty page and check that your entry is listed. Do not trust the terminal alone. The page is the source of truth for whether your entry is really in.

A few submission facts to keep in mind:

- **At most 5 submissions per UTC day, and 10 in total.** You do not have unlimited tries. Each submission counts, so make each one count.
- **The latest entry counts.** If you submit again, the newest entry replaces the older one. That is how resubmission works — see Step 6.
- **Exact ties go to the earlier receipt.** If two entries end up with exactly the same score, the one whose receipt came earlier wins the tie. Submitting early, when the entry is ready, is worth a little extra for exactly this reason.
- **Your repo must be public.** A private repo cannot be checked and cannot count. If you created it private by habit, change it to public before you submit — and check that the change actually took.
- **Your repo must be created after the competition opened.** A repo you made last month, or last year, does not qualify, however good the code in it is. For this bounty, that means created after 18 Nov 2026, 10:30 UTC.

Take your time on this step. A rushed submit with the wrong repo, the wrong commit, or missing transcripts is the most expensive kind of mistake, because it burns one of your limited submissions.

## 6. Check it, fix it, resubmit

After you submit, your entry gets checked. The checks verify that the repo is public, that it was created after the competition opened, that the license is there, and that the transcripts are real and match the code. If everything passes, your entry stands. If something fails, you get a message explaining what went wrong — and you get to fix it.

This is the step beginners fear most, and it is the step they should fear least. A failed check is not a rejection of your work. It is a specific, fixable problem with a specific fix. Read the message slowly. It usually names the problem directly: a missing file, a mismatched transcript, a repo that is still private, a license that is missing.

Here is the fix loop:

1. **Read the check message in full.** Do not skim it and guess. The message tells you what failed and often hints at what to do about it.
2. **Reproduce it locally.** Run the kit's `check` command on your machine. If it fails the same way, you can iterate quickly without burning a submission.
3. **Fix the actual problem.** If the repo is private, make it public. If the license is missing, add it. If the transcripts do not match, rebuild the mismatched part inside a recorded session so the transcripts cover it. Fix the cause, not the symptom.
4. **Run `check` again.** Keep fixing and re-checking locally until it passes.
5. **Resubmit.** Run the kit's `submit` command again with the fixed entry. Remember: the latest entry counts, so your fixed entry replaces the broken one. You have at most 5 submissions per UTC day and 10 in total, so do not resubmit blindly — resubmit only after the local check passes.
6. **Confirm again on the bounty page.** Make sure the new entry is the one listed, and that its status looks right.

Two things to watch out for in this loop:

- **Do not resubmit the same broken entry hoping for a different result.** The checks are deterministic — the same entry fails the same way. Fix first, then resubmit.
- **Do not burn submissions on guesses.** Each resubmit costs one of your 10 total, and at most 5 per UTC day. A local `check` is free. Use the free one to get it right, and spend the submission only when the local check passes.

If you are stuck on a check message you do not understand, re-read the task text and the kit instructions — the answer is usually there. If it is genuinely unclear, ask your agent to explain the message in plain language, then verify that explanation against the task text yourself before you act on it.

## 7. Claim your reward

If you win, you claim your reward from the on-chain escrow. The kit CLI has a `claim` command for this, and the `status` command tells you where your entry stands.

The flow is:

1. **Check your status.** Run the kit's `status` command, and look at the bounty page and leaderboard. Confirm that you are a winner and what place you came in.
2. **Claim with the kit CLI.** Run the kit's `claim` command. It claims your reward from the escrow to your keypair — the same Solana keypair that is your account and payout wallet.
3. **Verify the payout.** Check your wallet and confirm the USDC arrived. Keep a note of the amount, the date, and the place you came in. If anything looks wrong — the wrong amount, or nothing arriving — re-check the status first, then look for guidance on the bounty page before assuming the worst.

A note on timing: claiming happens after the competition ends and the results are final. For this bounty, the final check runs 30 hours after the deadline, so the provisional count you watch during the competition is not the final result. Do not try to claim before the results are final, and do not panic if the leaderboard moves during that final check — that movement is the point of the final check, catching signups that do not verify.

And a note on the referral rewards, which are separate from the bounty pool: you earn 0.25 USDC per signup your referral link brings, for the first 20 signups, plus a 10% share of what referred winners win for 90 days. Those rewards follow their own timing and rules on the platform — check your account page for how and when they are paid out.

## Worked example: your first bounty end-to-end

Theory is useful; a concrete run-through is better. Here is a full pass through the flow, using this very bounty as the example, with the real commands in order. Follow along in your head first, then do it for real with a bounty of your own choosing.

**The setup.** You have decided to enter bring-the-humans-02. The bounty opened 18 Nov 2026 at 10:30 UTC, entries close 21 Nov 2026 at 10:30 UTC (17:30 WIB), and the pool is $1,000 USDC across the top 50. Your plan: write a genuinely useful getting-started guide, publish it as a public repo, and share it with real people who want to try make.fun.

**Step 1 — Sign in.** Go to make.fun and sign in with your Solana keypair. Note your API key (`x-api-key`) — it lasts 30 days — and find your referral link. If you are following along with this guide as your way in, use mine to sign up:

**https://make.fun/r/19a3mn8a**

Code: `19a3mn8a`.

**Step 2 — Make a folder and get the kit.** Create a fresh folder for the entry, move into it, and download the kit for this bounty:

```sh
mkdir bring-the-humans-02
cd bring-the-humans-02
curl -sSL "https://make.fun/c/bring-the-humans-02/kit" | tar xz
```

Look at what landed. Read the kit's instructions. Work out what a passing entry looks like before you write a word.

**Step 3 — Build with your agent.** Open the folder in your AI coding agent and describe the entry in plain language. For this guide, the instruction was roughly: "Write a plain-English getting-started guide for a total newcomer to make.fun, covering account creation, picking a bounty, getting the kit, building, submitting, fixing failed checks, and claiming, plus a worked example, a mistakes section, and a troubleshooting table. Keep every fact true to the bounty page. Write it as a single README.md, and add an MIT license."

Work through it in small steps. Read each section as the agent writes it. Check the facts against the bounty page. Fix anything that sounds vague or that you cannot verify.

**Step 4 — Preview it locally.** Before you submit, read the guide the way a newcomer would. Serve the folder locally to see it rendered:

```sh
python3 -m http.server 8000
```

Open http://localhost:8000, read the guide start to finish, and note anything confusing, out of order, or wrong. Fix those things now, while fixing is cheap.

**Step 5 — Check locally, then submit.** Create your public GitHub repo — for this guide, owner `hesikafi`, repo name `bring-the-humans-02`, public, created after the competition opened, MIT license — and make one commit with the finished entry. Gather the agent session transcripts that wrote it. Then use the kit CLI, in this order:

```sh
node cli/makefun.mjs bundle
```

```sh
node cli/makefun.mjs check
```

`bundle` packages the entry up. `check` runs the checks on it, on your machine, before anything is submitted. If the check fails, fix what it names and run `check` again until it passes. Only then submit:

```sh
node cli/makefun.mjs submit
```

Then confirm on the bounty page that your entry is listed. Check its status whenever you want an update:

```sh
node cli/makefun.mjs status
```

**Step 6 — Share it with real people.** This is where the score for this bounty comes from. Share the guide — and your referral link — with people who genuinely want to try make.fun. Post it where newcomers actually ask how to start. Answer their questions. Help them through Step 1. Every verified human signup your link brings during the competition counts toward your score. Fake, bot, idle, same-person, same-network, and IP-cluster signups do not count, so do not try to game it — help real people instead, and the score follows.

**Step 7 — After the deadline, wait for the final check, then claim if you won.** Entries close 21 Nov 2026 at 10:30 UTC. The final check runs 30 hours after that. The provisional count you watched live is not the final result. Once results are final, check your status and, if you placed in the top 50, claim your reward from the escrow:

```sh
node cli/makefun.mjs claim
```

Then verify the USDC in your wallet. Keep a note of the amount, the date, and the place you came in.

That is the whole journey, end to end. Nothing in it requires experience you do not have — it requires care, in order, one step at a time.

## Mistakes that cost beginners a submission

These are the mistakes that turn a good entry into a failed check or a wasted submission. Most of them are boring, which is exactly why they are dangerous — nobody expects to lose an entry to a missing license.

- **Submitting a private repo.** The repo must be public. A private repo cannot be checked. Check the visibility on GitHub itself, not in your memory of what you clicked.
- **Reusing an old repo.** The repo must be created after the competition opened. An old repo with the new code pushed into it does not qualify. Create a fresh repo for each bounty.
- **Forgetting the license.** The repo must carry an OSI-approved license. This guide uses MIT. A repo with no license file fails the check, however good the rest of the entry is.
- **Submitting without running `check` first.** The local check is free and catches most problems before they cost you a submission. Skipping it is the most avoidable mistake in this whole guide.
- **Transcripts that do not match the code.** If you build something by hand after the agent session ends, or in a different tool with no transcript, the checks will notice the gap. Do the building inside recorded sessions, and submit the transcripts that cover it.
- **Building the wrong thing.** Read the task twice. Build what it asks for, in the format it asks for. A beautiful entry that answers a different question does not score.
- **Leaving submission to the last minutes.** Checks fail. Fixes take time. Resubmission takes a submission slot. An entry finished an hour before the deadline has room to fail a check and recover. An entry finished a minute before the deadline does not.
- **Burning submissions on untested fixes.** Each resubmit costs one of your 10 total, and at most 5 per UTC day. Fix locally, verify with `check`, and only then resubmit.
- **Sharing the private key.** Your keypair's private key is never part of a submission, a transcript, a screenshot, or a repo. If it appears anywhere public, stop and rotate it. (For this guide's author, the keypair never appears in the repo at all.)
- **Counting on signups that will not verify.** For this bounty, fake, bot, idle, same-person, same-network, and IP-cluster signups do not count, and your own account does not count. Chasing numbers with low-quality signups wastes effort that could have gone into helping real newcomers.
- **Trusting the provisional count as final.** The live count is provisional. The final check, 30 hours after the deadline, is what decides the score. Do not celebrate early, and do not despair early either — wait for the final check.

## Troubleshooting

When something goes wrong, start here. Find the symptom, read the fix, and try the fix before changing anything else.

| Symptom | Fix |
| --- | --- |
| `401` errors from the kit CLI, or commands that used to work suddenly fail | Your API key (`x-api-key`) lasts 30 days. If it has lapsed, sign in again on make.fun to get a fresh one, and make sure the kit CLI is using the new key. Do not keep retrying with the old key — a lapsed key will not start working again. |
| Entry refused: wrong repo owner | The submission must come from your own account and your own repo. Check that the repo owner on GitHub matches the account you signed in with, and that you submitted the repo you meant to — not a fork, not a teammate's repo, not an old repo under a different name. Fix the owner or the repo, then resubmit. |
| Badges still show as placeholders | Badges are generated from your entry once it exists on the platform. If they still show placeholder values, your entry may not be submitted yet, or the badge may be pointing at the wrong bounty slug, owner, or repo name. Check the bounty page to confirm your entry is listed, then check each part of the badge URL — slug `bring-the-humans-02`, owner, and repo name — character by character. |
| Session started before the bounty opened | The checks verify that the transcripts match the code and that the work belongs to this bounty. A session that started before the bounty opened cannot show work done for this bounty. Start a fresh agent session after the bounty opens, do the build inside it, and submit that session's transcripts. Do not try to reuse an older session. |
| Entry refused, and you are not sure why | Read the refusal message in full — it names the problem. Then run the kit's `check` command locally and read its output the same way. The message usually points at one of the common causes: a private repo, a repo created before the competition opened, a missing license, or transcripts that do not match the code. Fix the named cause, re-run `check` until it passes, and only then resubmit. Remember the limits: at most 5 submissions per UTC day, 10 in total, and the latest entry counts. |
| Kit download fails | Check the slug first — for this bounty it is `bring-the-humans-02` — and retype the kit command carefully, or copy it from the bounty page. Make sure you are in an empty folder. If it still fails, check your network, then re-read the bounty page for the kit link. |
| You cannot sign in | Check that you are using the right keypair. If you have more than one, you may be signing in with the wrong one. Make sure you can sign in and out cleanly before the deadline, while you still have time to sort it out. |
| The leaderboard count moved after the deadline | That is expected. The live count is provisional, and the final check runs 30 hours after the deadline. Only the final check decides the score. Wait for it before drawing conclusions. |

If your symptom is not in this table, go back to the check output and the task text. Between them, they almost always name the problem. And remember: the local `check` is free. Use it as often as you like.

## Or let your agent do the whole thing

You have read this guide. Now here is the honest shortcut: you can hand this whole guide to your AI coding agent and let it do the work.

That is, after all, how this guide was built — and how make.fun expects entries to be built. The platform is designed for agents doing the building, with humans directing, checking, and deciding. You do not have to type every word yourself. You have to direct clearly, check honestly, and take responsibility for the result.

Here is a prompt you can give your agent, adapted from the one used for this guide:

> Build an entry for the make.fun bounty bring-the-humans-02, "Bring the humans again". Write a plain-English getting-started guide for a total newcomer to make.fun, as a single README.md, plus an MIT license file. Cover: what make.fun is and how a bounty moves from open to paid, what the newcomer needs before starting, then steps for creating an account, picking a bounty, getting the kit, building, submitting, fixing failed checks, and claiming. Add a worked end-to-end example with the real commands, a mistakes section, and a troubleshooting table. Include the referral link https://make.fun/r/19a3mn8a with code 19a3mn8a near the top, in Step 1, and in a closing referral section. Keep every fact true to the bounty page. Use the run command `python3 -m http.server 8000` for local preview. Do not invent numbers, dates, commands, or program details.

Then do the human part:

1. **Read what it wrote.** All of it. End to end. You are the author now — if a step is wrong, it is your entry that fails.
2. **Check the facts.** Every number, date, command, and claim against the bounty page. The agent can get details wrong with total confidence. Your job is to catch that.
3. **Run the checks.** Use the kit's `check` command locally before you submit anything.
4. **Submit, and share with real people.** For this bounty, the score is verified human signups — so the sharing is the work, not an afterthought.

Letting your agent do the whole thing does not mean skipping the thinking. It means moving the typing to the agent and keeping the judgement for yourself. That is the deal make.fun is built on: agents build, humans direct and verify.

## Earn with your own referral link

Once you have an account, you have your own referral link — the same shape as mine, with your own code. Sharing it is how you earn beyond the bounty pool itself.

Here is how the referral rewards work:

- **0.25 USDC per signup**, for the first 20 signups your link brings.
- **A 10% share of what referred winners win**, for 90 days. If someone who signed up through your link goes on to win a bounty, you earn 10% of their winnings for 90 days.

And here is how it works for this bounty specifically:

- **Your score is the number of verified human signups your referral link brings during the competition.** The provisional count shows live; the final check runs 30 hours after the deadline. Fake, bot, idle, same-person, same-network, and IP-cluster signups do not count, and your own account does not count.

So the way to earn — in this bounty and in general — is the same: help real people get started, and share your link where that help actually lands.

### Before you share

Run through this short checklist first, so the link you share leads somewhere worth landing on:

- Your guide is finished, and you have read it end to end as a newcomer would.
- The referral link in it is your own, and you have clicked it once to confirm it opens the right page.
- You can answer the first question a newcomer will ask — usually "what do I need to start?" — without sending them back to the guide for it.
- You are sharing it where people are already asking how to start, not dropping it into a conversation where nobody asked.

A few practical notes on sharing well:

- **Share the guide, not just the link.** A bare link with no context looks like spam and gets ignored. A guide that actually helps someone get from zero to a first submission gives them a reason to click, and a reason to stay.
- **Go where newcomers ask questions.** If someone is asking how to start with make.fun, that is the moment your guide is useful. Answer their question first, then share the link as the next step.
- **Help them through Step 1.** The biggest drop-off is account creation — the keypair, the sign-in, the API key. If you help someone past that step, they are far more likely to finish, and a finished newcomer is a verified signup.
- **Do not buy, fake, or farm signups.** It does not work — the final check catches it — and it wastes the effort you could have spent helping real people. Twenty genuine signups beat two hundred that do not verify.
- **Use your own link once you have one.** My link got you here:

**https://make.fun/r/19a3mn8a**

Code: `19a3mn8a`.

Once you are signed up, share *yours* the same way — with a guide, with help, with real people. That is how the referral system is meant to work, and it is how this bounty is scored.

## Questions

Common questions, answered briefly. Click a question to expand it.

<details>
<summary>Do I need to know how to code?</summary>

Not to follow this guide, and not to build every kind of entry. You build with an AI coding agent, which does the typing. What you need is the ability to read the task, direct the agent clearly, and check the result honestly. If you can do that, you can enter.
</details>

<details>
<summary>Do I need to know Solana or smart contracts?</summary>

No. You need a Solana keypair to sign in — that is your account and payout wallet — but you do not need to write a smart contract or build a Solana app. The escrow and the claiming are handled by the platform and the kit CLI.
</details>

<details>
<summary>Is my reward really locked before I start?</summary>

Yes. The whole reward for a bounty is locked in an on-chain escrow on Solana when the bounty opens. That is the point of the escrow: the money is set aside for this bounty, and winners claim from it.
</details>

<details>
<summary>What do I submit, exactly?</summary>

A public GitHub repo at one commit, plus the AI session transcripts that wrote the code in it. The repo must be public, created after the competition opened, and carry an OSI-approved license. The checks verify that the transcripts are real and match the code.
</details>

<details>
<summary>How many times can I submit?</summary>

At most 5 submissions per UTC day, and 10 in total. The latest entry counts, so a resubmission replaces your previous entry. Exact ties go to the earlier receipt, so submitting a good entry early is worth a little extra.
</details>

<details>
<summary>How long does my API key last?</summary>

30 days. It is labelled `x-api-key`. If your kit commands suddenly start failing with 401 errors after working fine, a lapsed key is the first thing to check — sign in again to get a fresh one.
</details>

<details>
<summary>What counts toward my score in this bounty?</summary>

The number of verified human signups your referral link brings during the competition. The provisional count shows live, and the final check runs 30 hours after the deadline. Fake, bot, idle, same-person, same-network, and IP-cluster signups do not count, and your own account does not count.
</details>

<details>
<summary>When does this bounty close?</summary>

Entries close 21 Nov 2026 at 10:30 UTC (17:30 WIB). The bounty opened 18 Nov 2026 at 10:30 UTC. Do not leave submission to the last minutes — leave time for a failed check and a fix.
</details>

<details>
<summary>What if my entry fails the checks?</summary>

Read the message in full, run the kit's `check` command locally, fix the named cause, re-run `check` until it passes, and then resubmit. A failed check is a fixable problem, not a rejection of your work. See Step 6 for the full loop.
</details>

<details>
<summary>Can I earn without winning the bounty?</summary>

Yes, through referrals. You earn 0.25 USDC per signup your link brings, for the first 20 signups, plus a 10% share of what referred winners win for 90 days. See the referral section above for the details.
</details>

## Links

- **make.fun** — https://make.fun/
- **This bounty (bring-the-humans-02)** — https://make.fun/bounty/bring-the-humans-02
- **Leaderboard for this bounty** — https://make.fun/bounty/bring-the-humans-02/leaderboard
- **My referral link** — https://make.fun/r/19a3mn8a (code `19a3mn8a`)
- **skill.md, guides, Discord, and X** — find these from the make.fun site and the bounty page. I have not listed direct links for them here, because I would rather point you to the source than guess a URL that might be out of date. Start at https://make.fun/ and follow the links from there.

## About this guide

This guide was written for the make.fun bounty bring-the-humans-02, "Bring the humans again". Its facts were checked on 20 Nov 2026, and the numbers in it — the $1,000 USDC pool, the top-50 split, the dates, and the entry count — are a snapshot from that day. If you are reading this later, check the bounty page for the current numbers, because pools, dates, and entry counts move. The steps, though, are the shape of how make.fun works: sign in with a Solana keypair, pick a bounty, get the kit, build with an AI agent, submit a public repo with its transcripts, fix what the checks flag, and claim from the escrow if you win.

<sub>Entered on [make.fun](https://make.fun/?ref=19a3mn8a&utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02) · AI agents build software for cash rewards</sub>
