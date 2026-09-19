# Your books

*My year-end still goes to a professional. This is the setup for the other eleven months, written so the professional isn't cleaning up after you in April.*

## What this does for a shop

Claude can connect straight into QuickBooks Online, through Intuit's own sign-in, so Claude never sees or holds your QuickBooks password. Once it's connected, Intuit says it can pull a profit and loss report, show your cash flow, tell you who owes you and which of your own bills are due, compare your numbers against others in the trade, pull in transactions, and create, update, and send invoices and estimates.

Here's a real use for it. Say it's the end of the month and something's off: the bank balance in QuickBooks doesn't match your real bank balance, but you don't know why yet. The prompt at the bottom of this chapter tells it to start every session by pulling this month's numbers against last month's, listing everything still uncategorized, and comparing the QuickBooks balance to the real bank balance, and to show you the difference rather than fix it. You still decide what to do about it. The point is getting to the actual problem faster than clicking through screens yourself.

## What it costs, honestly

As of September 2026, connecting QuickBooks doesn't cost anything beyond your Claude plan (the free plan includes connectors) and whatever you already pay Intuit for QuickBooks Online. The connector is US only as of September 2026.

Time cost: a few minutes to connect it the first time, and then whatever time you spend reviewing what it did, which is the real cost of any of this, not the connecting. Year-end tax work still goes to a professional. That's my rule, not a suggestion.

## What you need before you start

- A Claude account. Connectors are part of every plan; whether the QuickBooks one shows a Connect button on the free plan is what step 2 tells you
- A QuickBooks Online account and your Intuit login
- About ten minutes, and a clear head, for the first connect

## Step by step

1. In the Claude app, open Connectors in the left navigation.
2. Find QuickBooks in the list and choose Connect.
3. You'll be sent to Intuit's own sign-in page. Sign in there with your Intuit login, not a Claude password. Claude never holds your QuickBooks password.
4. If there's no Connect button next to QuickBooks at all, that means your current plan doesn't include it. That's the answer, don't guess further, check the plan page instead.
5. Once it's connected, start a brand new chat.
6. Paste the block below as your very first message, filling in your shop name and today's date.
7. Read what it says back before you do anything else. It should tell you what it can see and what it can't, not launch straight into changing something.

Paste as the first message in a new Claude chat (or a new Claude Code session on a paid plan), with your shop name and today's date filled in:

```
You are the bookkeeper for [SHOP NAME], a small appliance repair company that runs QuickBooks Online. I'm the owner, not an accountant. Work like a careful bookkeeper, not a salesman.

Rules:
1. Never invent a number. If you don't have it, say what you need and where I'd get it.
2. Read before you write. Start every session by pulling this month's P&L against last month, the A/R aging, the bank balance in QuickBooks against the real bank balance, and every uncategorized transaction.
3. Read-only until I say otherwise. Before you create, change, or delete anything in QuickBooks, show me exactly what you're about to do and wait for my yes.
4. Categorize by my rules, not your guess. If a transaction could go two places, ask me once and remember the answer.
5. Reconcile to the bank every month. If QuickBooks and the bank don't match, the bank is right until proven otherwise. Find the difference and show me.
6. Anything about taxes, payroll, sales tax, or what's deductible: give me your best read, then say "confirm with your CPA" every time. You are not my tax professional.
7. Plain English. No accounting words without a one-line explanation the first time.
8. End every session with three things: what changed, what you're not sure about, and what you need from me.
9. Keep a running list called OPEN QUESTIONS and read it back to me at the start of the next session.
10. Passwords and bank logins never go in this chat. If I paste one by mistake, tell me to change it.

Today's date is [DATE]. My fiscal year is the calendar year. Start by telling me what you can see and what you can't.
```

## What goes wrong first

1. There's no Connect button at all. Check your plan instead of hunting for a setting that isn't there.
2. The Intuit sign-in screen looks like nothing happened right after you log in. Give it a moment to redirect you back to Claude.
3. It offers to change or categorize something in QuickBooks before you've told it your rules. Don't approve it yet, reread rule 3 in the prompt above.
4. It hands you a number that sounds right without saying where it came from.
5. You approve a change because it looks reasonable, without actually reading what it said it was about to do, which is the one habit the whole prompt above is built to stop.

## What I'd do

Use the prompt above word for word the first few times, don't shortcut it. Keep it read-only until you've watched it work through a full month and you trust what it's finding. The moment anything touches taxes, payroll, or what's deductible, treat its answer as a first draft and confirm with your CPA, every time, no exceptions.

---

[Back to the front page](README.md) · [Next: What goes wrong](04-what-goes-wrong.md)
