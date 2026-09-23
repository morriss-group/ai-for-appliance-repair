# Your phone, answered

*It answers my line today. It got there on real calls, not demos, and every change still goes onto a second number before it touches the one customers call.*

## What this does for a shop

This is a phone number that answers itself. A caller says their washer is leaking, the agent asks what's wrong, gets their address, checks whether you cover that area, looks at your actual calendar, offers real open windows, and books the appointment. Mine knows my service area by ZIP code, and inside the ZIPs I only partly cover, by neighborhood, so it declines the far side of a ZIP the same way I would, politely, before anyone's time is spent. You find out when it lands on your schedule. It talks like a person having a conversation, not a phone tree where someone presses 1 for service.

The problem it solves is that I can't answer the phone with my hands inside a machine. Now a call at 9 PM, on a Sunday, or while I'm on my back behind a dryer gets answered and booked onto my calendar, and I read the recording later.

**It says it's recorded before they say a word.** Mine opens every call with the same two facts: it's an AI receptionist, and the call is recorded. You have to set that up yourself, and it has to come before the caller speaks, not after. Then every call lands in my email as a transcript, with the recording attached, so if a customer says they were told something, I can listen to what was actually said. That's the only reason I can trust a machine to answer my phone: I can check it.

**Where the rules live.** The words you type into the voice platform are the agent's manners: how it greets, what it asks, how it says no. They are not where the rules that matter live. Mine has forgotten a prompt rule three times in one week, because a long prompt is a suggestion the model weighs against everything else the caller says. It has never once booked a holiday, offered a window I don't work, or booked outside my area, because those aren't sentences in the prompt. They're a small program on a server that the agent has to ask before it can book anything, and the program says no and can't be talked out of it. If you build this, put every rule you'd fire a dispatcher for breaking in the code, and leave the prompt for the manners.

**Yours, or the one your CRM sells you.** That's the difference between a voice agent you build and the one that comes bundled with your CRM. On the bundled one you don't get to make those customizations. What Housecall Pro's own pages say you can change on theirs, as of September 2026: your scripts, your hours, your business details, and the escalation and forwarding rules. What you can't touch: the booking logic, the calendar rules, anything about your area finer than a ZIP, and anything that lives in code. So it won't learn the neighborhoods inside a ZIP you only half cover, and when it does something you don't like, you file a complaint and wait. On yours, the rule is a line in a program you can read, and you change it the same afternoon. In my experience yours also costs a lot less to run, and here are the numbers I can actually stand behind, as of September 2026. Housecall Pro's bundled agent, CSR AI, has no public price; it's "contact us" on their pricing page, and the one trade-site estimate I found puts it at $200 to $500 or more a month, which I can't verify. Mine runs on a voice platform that bills per call: the review log for this month shows a median of 11 cents a call and about $8.50 across every call it priced, plus a few dollars for the phone number and a small server. One honest catch if your CRM is Housecall Pro: booking onto your calendar needs their API, and API access is on their Max plan only, $299 a month billed annually. If you're already on Max, yours is cheaper by a wide margin. If you're on a lower plan, count the upgrade before you count the savings.

And the rule underneath all of it: if your CRM won't give you API access to your own schedule, on any plan, and you want a good voice agent, find another CRM. A voice agent that can't write to the calendar is a message-taker with a nice voice. A CRM is also smaller than it looks from the price tag, a calendar, a customer list and an invoice, and for a shop that won't pay a Max plan for one, a custom one can be built. I've built one for a bike shop and I'm rebuilding it now. That's a thing I can do, not a thing this guide teaches.

**Some people will hate it, and they'll say so where it counts.** I have the proof: two one-star reviews on my business, both for the voice agent and nothing else. One of them accused me of cussing her out on the phone. The call was recorded, so I know what was and wasn't said; the review is up anyway, and it counts the same as any other. That's a real cost, and it's the one nobody puts in the sales pitch. Part of it is that people hear "AI" and picture the phone tree they've been fighting for twenty years, press 1 for service, and hang up angry before they find out this one isn't that. This one works the way a person does: it's on the phone with the caller and on the computer at the same time, checking the real calendar while it talks, and it books the job. Most callers figure that out in the first thirty seconds. A few never will, and they'll leave a review. Decide now that you can live with that, because you can't turn it off for the people who'd hate it.

**What it did to the numbers, measured.** I projected the phone agent would add 25 percent. On September 19, 2026, I pulled completed-job revenue out of my CRM and compared the six weeks since it went live, August 9 to September 18, against the same six weeks in each of the two years before. Up 56 percent on 2025 and 62 percent on 2024, on a third more completed jobs and an average ticket up 18 percent. The six weeks right before it went live were up 11 percent on 2025; the six weeks after, 56. August alone was up 36 percent, and the first half of September 97. Those same weeks had been flat from 2024 to 2025, so it isn't the season. Year to date the whole shop is 14 percent over 2025 and 31 percent over 2024, because the agent has only been on the line for six of those weeks. Two things are inside the six-week number and I can't separate them: the phone getting answered every time, and the chapter 1 pricing rules raising the ticket. Six weeks is six weeks. The winter number goes here when I have it, whichever way it goes.

## What it costs, honestly

This is the hardest of the three things in this guide to set up. Figure on an afternoon to get it standing up, and then more time after that tuning it against real calls, because a scripted test call is not the same as a real customer talking over your agent or mumbling an address.

The build has its own honest cost breakdown covering three separate charges: the voice platform, the phone number, and the voice itself. I'm not going to repeat numbers here that change on their own pricing pages. Read the real breakdown before you commit to anything: see "What it costs, honestly" in [START-HERE.md](https://github.com/morriss-group/vapi-voice-tuneup/blob/main/START-HERE.md).

## What you need before you start

- A VAPI account, or a similar voice platform
- A second phone number bought through Twilio and imported, not a number the voice platform gives you (a platform-provided number may not be able to transfer a call to a person)
- Your business rules written down: hours, service area, brands you decline
- If you want it booking onto your real calendar, your scheduling software's own API access

## Step by step

1. On your phone or computer, open the repository at [github.com/morriss-group/vapi-voice-tuneup](https://github.com/morriss-group/vapi-voice-tuneup). Never used GitHub? [How this works, and what to click](how-this-works.md) first.
2. Open START-HERE.md and read the whole page. It's plain English, about five minutes, and it will tell you honestly whether to build this yourself, hand it to your tech person, or skip it entirely.
3. If you're building it yourself, follow the link inside START-HERE to README.md for the setup steps in order, most impactful fix first.
4. Stop here if you're on a phone. Everything from this step on needs a computer with a terminal, and the kit's deploy guide says which one and how. If you don't have that, hand the kit link to your tech person and skip to step 6.
5. Set up a VAPI account and buy a second phone number through Twilio, not through VAPI. Three meters start here and the kit's START-HERE names every one of them: the voice service, the phone number, and the hosting, plus your scheduling software's plan if you want it booking onto your calendar.
6. Work through DEPLOY-GUIDE.md in the same repository to stand up your assistant on that second number.
7. Call your new number yourself, at night, more than once, before you connect it to your calendar or tell anyone it exists.
8. Once it sounds right on the test number, MAKE-WEBHOOK-WALKTHROUGH.md gets you a report of every call in your inbox. That is a report, not a booking. Booking onto your real calendar is Layer 4 of DEPLOY-GUIDE.md, and the example tool in the kit is a placeholder that must never be attached to a live number.
9. Before you leave the repository page, click Watch, then Custom, then Releases. That is the only way GitHub will ever tell you a fix was published. I keep fixing this thing as real calls show me what is wrong, and a copy you downloaded does not update itself. Every fix is listed in CHANGELOG.md with the exact line to change in yours.

## What goes wrong first

1. The voice sounds flat or robotic, or there's a long pause before it answers you.
2. It talks to a voicemail greeting like it's a person and says something confusing to the machine.
3. It reads a phone number or an address back as a string of digits instead of speaking it the way a person would.
4. You skip the test-number step and point it at your real business line too soon.
5. A caller who hates talking to a machine leaves a one-star review that says nothing about the repair. Read the recording before you reply. Reply once, plainly, and don't argue.
6. It works fine on every test call, and then the first time it needs to transfer a real caller to you, the transfer silently fails, because the number came from the voice platform instead of Twilio.

## What I'd do

Get the second number first, and don't skip that step. Live with it for a couple of weeks. Call it yourself, let it book fake appointments, listen back to the recordings. Your phone line is your income, and this build is set up to earn your trust slowly on purpose. If the words "API key" make you want to close the laptop, that's a fine answer, hand the whole repository to whoever does your tech instead of building it yourself.

---

[Back to the front page](README.md) · [Next: Your books](03-your-books.md)
