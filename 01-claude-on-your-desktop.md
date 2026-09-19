# Claude on your desktop

*I send it a nameplate photo most days now, from under the machine, and I check its answer before I order.*

## What this does for a shop

Claude is a chat program. You type to it, talk to it, or show it a photo, and it writes back in plain words. On a computer it's at claude.ai. On a phone it's the Claude app from the App Store or Google Play, or the same website in your browser. Either way, you're having a conversation, not running a program with menus and buttons to memorize.

Here's how I actually use it, every day, on real jobs. It helps me diagnose. It helps me look up parts. It finds the published average labor for a repair so I can sanity-check my own rate. It prices the part the way I price parts, retail plus tax plus fifteen dollars shipping, rounded to the nearest five, because that's my markup and I told it so once. Then it writes the two lines I put on the ticket: a labor line that describes the whole repair in plain words the customer can read, and a part line with the part number and the price. I read both, fix anything that isn't how I'd say it, and paste them in.

It will do whatever you tell it to do. If you mark up from wholesale instead, or you follow a chart for your markup like a lot of shops do, it will follow the chart. You just have to let it know what it needs to do, once, in plain words.

One rule I don't bend: I don't order off its part number. I take the number it gives me to a parts website and check it against the real listing first, because it can be wrong, and a wrong part costs me a wasted trip. That check takes two minutes.

## What it costs, honestly

As of September 2026, Claude has three plans. Free costs $0 and includes connectors (more on those in chapter 3), but not Claude Code. Pro is $20 a month, or $17 a month if you pay for the year up front. Max starts at $100 a month. For everything in this chapter, the free plan does the job.

Time cost: about ten minutes to sign up, and each of the three jobs below takes less time than it would to look the answer up yourself.

## What you need before you start

- A phone or computer with a camera
- An email address to sign up with
- About ten minutes with no interruptions, the first time

## Step by step

1. On your phone, open a browser and go to claude.ai, or install the Claude app from the App Store or Google Play. Look for a button that says something like "Sign up" or "Get started."
2. Enter your email (or sign in with an existing Google account) and follow the prompts. You should land on a chat screen with a blank message box at the bottom.
3. Before anything else, find Privacy Settings and turn off the switch that lets your chats be used to improve Claude. Off means your chats are kept 30 days and not used for training.
4. Now the real job. Paste this as your first message, with your own numbers filled in. It tells Claude how you price, once, so you never explain it again in that chat:

```
I run an appliance repair shop. When I give you a nameplate photo and a symptom, do these in order:
1. Tell me the model and what part most likely failed, and say how sure you are.
2. Give me the part number and tell me to verify it on a parts website before I order.
3. Find a current retail price for that part and the published average labor for this repair, and say where each number came from.
4. Price the part my way: retail plus [YOUR TAX RATE]% tax plus $15 shipping, rounded to the nearest $5. My labor for this kind of repair is $[YOUR RATE].
5. Write two line items for my ticket. Line one, labor: describe the whole repair in plain words a customer can read, with the diagnosis. Line two, the part: part number, what it is, and the price.
Never invent a price or a part number. If you can't find one, say so.
```

5. Take a photo of the nameplate, tap the small icon near the message box (a camera, a paperclip, or a plus), attach it, and type the symptom the way the customer said it.
6. Read the answer. Then open a parts website in another tab and check the part number against the real listing before you buy anything.
7. Read the two line items out loud. Change anything that doesn't sound like you. Then paste them into your ticket and send.
8. Do a real job with it the same day you set it up, not next week. Finishing something small the same day is what makes it stick.

In my shop it goes one step further: it writes those lines straight into Housecall Pro for me, on the job, and I never paste anything. That takes Claude Code, a paid plan, and a key from Housecall Pro. That's [chapter 5](05-your-crm-and-the-shops-memory.md).

## Set it up once, so every chat knows your shop

Step 4 taught one chat how you price. The next time you open Claude and start a new chat, that chat has never met you. It doesn't know your tax rate, your labor rate, or that you run an appliance repair shop, and it will happily price a job some other way. Claude does keep a memory of you now, and it helps, but it's a summary, and it won't go read your old chats unless you ask it to (and searching old chats is a paid-plan feature anyway). Don't lean on it for your pricing rules. Put them where every chat reads them before you type a word.

Do this once. It takes two minutes.

1. On the website, click your initials in the lower left corner and choose Settings. In the phone app the same Settings is behind the menu, under your name. Either way, look for the box labeled "Instructions for Claude."
2. Paste the pricing prompt from step 4 into that box, with your numbers filled in, and add one line at the top: "You work for one appliance repair shop, mine. Everything I ask you is about running it." Save.
3. Test it. Start a brand-new chat, send a nameplate photo and a symptom, and see whether it prices your way without being reminded. If it doesn't, the box didn't save. Go back and look.

One step further, and it's on the free plan too: Claude has Projects, up to five on a free account. A project is a folder of chats that all share the same instructions and the same files. Make one with your shop's name on it. On the left side of the screen tap Projects, then "+ New Project," then "Set project instructions," paste the same prompt, and save. Start every shop chat inside that project. The one thing a project won't do is carry a conversation across chats: what you told one chat inside the project, the next chat inside it hasn't heard, unless you saved it to the project's knowledge. So a rate you typed into a message is gone tomorrow. A rate you typed into the instructions is there every time.

And in the middle of a job, stay in the chat you started. Don't open a new one for your second question about the same machine. The new one hasn't seen the photo.

## What goes wrong first

1. You take a bad photo, glare, blur, or half the label cut off, and get a bad answer back. Retake it in better light.
2. You accept the part number without checking it and order the wrong part. It happens; that's why step 6 exists.
3. You give it the symptom in your words instead of the customer's, and it diagnoses your guess instead of their problem.
4. You send the drafted text straight to the customer without reading it, and it says something you wouldn't say.
5. You try it once, get a decent answer, and never open it again, because nothing forced you to build the habit.
6. You set it all up in one chat, come back the next morning in a new chat, and it acts like it never met you. That's the section above. Do it once and this stops.

## What I'd do

Start with the nameplate photo. It costs nothing to try, and you'll know inside a minute whether it's useful to you. Do the check-the-part-number step every single time for the first month, even when you're sure, until it's automatic. Once that's a habit, decide for yourself whether the $20-a-month plan is worth it. I wouldn't pay for anything on day one.

---

[Back to the front page](README.md) · [Next: Your phone, answered](02-your-phone-answered.md)
