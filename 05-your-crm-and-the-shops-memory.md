# Your CRM, and the shop's memory

*I don't write tickets or look up parts anymore. I take a picture of the model number and the tech sheet, tell it what the customer said, and read what it writes before it goes on the job.*

## What this does for a shop

This is the step past chapter 1. In chapter 1 Claude writes the two line items and you paste them into your ticket. In this chapter it has a key to your CRM, so when you say "write up the ticket," it writes the ticket. The labor line with the whole repair in plain words, the part line with the number and the price, and a note on the job with the model, the serial and what you found. You read it, you say yes, it's on the job.

The second half is memory, and the order matters. I photograph the model number first. If it already has the tech sheet for that model, we go. If it doesn't, I photograph the document, whatever the maker calls it: the tech sheet, the mini manual folded inside the door or behind the kick plate, the wiring diagram, or the full service manual, or I download it from the makers who give them out, and it gets filed by model with the fault codes, the service mode, the test points and the wiring typed out. If there's no sheet to be found, it still helps, but noticeably less. The document is what makes it good. With the document in front of it, it's a tech line: it has the sheet, it has what failed on that model last time, and it never puts you on hold. Whether it beats the manufacturer's tech line is my opinion, not a measurement, and my opinion is yes.

This morning that was a GE dishwasher with an intermittent dead display: hold the left pad and Start five seconds, count the blinks, eight blinks is a stuck key, and the service light on the main board under the tub tells you whether it's the panel or the board. That's off the sheet, in plain words, before I had the door apart.

It will not fix the appliance for you. What it does is get a tech close, and tell them what to check next, the way you would if a green tech called you from the customer's kitchen and you were talking them through it. Status, honestly: the tickets and the tech-sheet filing are in use, every day. The memory across visits is a month old and growing. A new hire has not run on it yet, because I'm one truck. That last part is what I expect, not what I've measured.

## What it costs, honestly

As of September 2026 this needs a paid Claude plan, because it runs in Claude Code, which the free plan doesn't include: Pro at $20 a month, or Max from $100 if you use it all day. Your CRM has to offer API access, and some only do on their higher plans; on Housecall Pro it's a setting on the higher tiers, and I won't quote which, check your own plan page. Time cost: an afternoon to set up, then it saves you the ticket-writing on every job after that.

## What you need before you start

- A paid Claude plan and Claude Code installed on a computer. Chapter 1 put the Claude app on your phone; Claude Code is a separate install on a computer, from Anthropic's Claude Code page, and it needs the paid plan.
- A CRM that gives you an API key, and the key
- One folder on your computer for the shop, with three things in it: your pricing rule from chapter 1, a folder for tech sheets, mini manuals, wiring diagrams and service manuals, and a text file that will become your ledger of what failed and what fixed it
- The rule in writing, before the key goes anywhere: it shows you the ticket and waits for your yes, every time
- A computer at the house that stays on, for the teaching half. You can use Claude from the phone all day with nothing at home switched on; chapter 1 is exactly that, and it's most of what you'll do in the field. What needs the computer at the house is teaching it: filing a tech sheet, writing the ledger, writing to your CRM. Those live in the shop folder with the key and the memory, so the phone in the truck is the window and the desktop at the house is the hands. Mine is a desktop and a Linux box, both on all the time. Change the sleep settings so the desktop never sleeps, plug it into a power strip nobody switches off, and count the electricity as part of the cost.

**If you don't have a CRM.** You don't need one to start this chapter. The shop folder, the RULES file, the tech sheets and the ledger work exactly the same with no CRM at all; the only step that changes is where the finished ticket lands. Claude's Google Calendar connector can put the job on a calendar it can see, and on a Mac, Claude Code can write to Apple Calendar and Apple Reminders. I run Housecall Pro, so that isn't what runs in my shop; it's what the tools do, and it's where I'd start if I weren't ready to pay for a CRM. Move to one when you've got a second tech, or when you're tired of typing invoices by hand.

**The five percent.** If you have a CRM and you don't like it, you don't have to keep using the parts you don't like. If you don't have one and you want one, buy it for the five percent you'll actually use and let the system run that five percent. Nobody uses all of a CRM, and everybody pays for all of it. My guess, and it's a guess from years of paying for one, is that most shops use five to ten percent of what they bought, and every shop uses a different five to ten percent. That's why nobody can build the right software for you until they know which five percent you use, and that's the one thing you know better than any software company. Now you can build your own five percent. Write down the five screens you actually open in a week. That list is the spec, the RULES file is the rest, and the AI does the building. I'm testing that on my own shop right now, and it isn't running my business yet, so this paragraph is a belief and a plan, not a report.

## Think it out in the chat first

The chat app and Claude Code are two different tools, and I use them for two different jobs. The chat is where I think. Claude Code is where things get built and changed. The chat can't touch anything, so it's the safe place to be half-right out loud. Claude Code has its hands in your files and, in this chapter, in your CRM, so by the time you open it you want to know exactly what you're asking for.

So the habit is: bounce the idea off the chat, then have the chat write the brief.

1. Open a chat (inside your shop project, if you made one in chapter 1) and say what's bugging you, in your own words. "I lose twenty minutes a job writing tickets." "I can never find the tech sheet for a model I know I've seen." Talk it through. Make it argue back: "tell me why this is a bad idea" gets you more than "is this a good idea."
2. When you can say in two sentences what you want and what done looks like, ask it to write the brief. Paste this:

```
Write a brief I can hand to Claude Code to build this for my shop. One page. Use these headings: What I want. What done looks like. What you must not touch. What I already have. Questions to ask me before starting. Plain words, no code. If anything I've said contradicts itself, say so at the top.
```

3. Read the brief. Cross out anything that isn't true about your shop; the chat guesses at what you have, and you don't have to guess. If it lists a question for you, answer it in the brief before the brief goes anywhere.
4. Open Claude Code in the shop folder, paste the brief, and say: "Read this. Tell me what you'd do and what could go wrong, before you change anything." Let it ask its questions. Then say go.

I go one step further. I hand the same brief to a second chat, sometimes one from a different company, and tell it to tear the brief apart before Claude Code ever sees it. Two models that never saw each other's work agreeing on something is worth a little. One model agreeing with itself is worth nothing.

## Step by step

1. Make the shop folder. Call it your shop's name. Inside it, make a folder called tech-sheets and an empty text file called ledger.
2. Put your chapter 1 pricing prompt in a file in that folder called RULES, and add two lines to it: "Before you create or change anything in my CRM, show me exactly what you're about to write and wait for my yes." and "Never put my API key in a chat or a file you show anyone."
3. Get your API key from your CRM. It's a long string of letters and numbers. Put it in a file the agent can read but that never leaves your computer; Claude Code will tell you how when you ask it "where should my CRM key live so it's never in a chat."
4. Open Claude Code in the shop folder and tell it, in plain words, what the folder is: "This is my shop. RULES is how I price and how you behave. tech-sheets is where model sheets go. ledger is where you write what failed and what fixed it, one dated entry per job."
5. First job. Photograph the nameplate and the tech sheet, drop both in, and tell it what the customer said. Ask what to check first. Read what it says against the sheet in your hand.
6. When you've found the fault and the part, say "write up the ticket for job [number]." It should show you the two lines and the note, then stop. If it writes without showing you, stop right there and fix RULES before anything else.
7. Say yes. Open the job in your CRM and read what landed. Do this on every job for the first month, not just the first one.
8. Ask it to file the tech sheet by model and write the ledger entry. Next time you're at that model, ask "what do we have on this one" before you open the door.

## What goes wrong first

1. The key ends up in a chat. If it does, go to your CRM and make a new key, then delete the old one.
2. It writes to the wrong job. Always give it the job number, and read what landed.
3. The tech sheet photo is unreadable, and it fills the gaps with what it thinks a sheet like that would say. Retake the photo. Ask it to mark anything it couldn't read.
4. It "remembers" a model you've never had it file, because it's guessing from a similar one. Ask it which file it read. If it can't name one, it didn't read one.
5. You stop reading what it wrote, because it's been right all week. The week you stop reading is the week it puts a wrong part number on a real ticket.

## What I'd do

Keep it to ticket writing and tech sheets for the first month, with the show-me-first rule in writing, and read every line it puts on a job. Don't hand it the phone, the calendar or the money until you've caught it being wrong once and seen how it handled being corrected. And if you're thinking about a new tech: put them on it the first week, but you read every ticket they let it write. The system gets a green tech close. It doesn't get them there.

---

[Back to the front page](README.md) · [Next: One truck to five](06-one-truck-to-five.md)
