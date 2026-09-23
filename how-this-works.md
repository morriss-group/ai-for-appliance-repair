# How this works, and what to click

*For the guy reading this on his phone in the truck. You don't need an account to read any of it. You need one, free, for exactly two things, and both are spelled out below.*

## What "open source" means here

I built a phone agent and a set of instructions for my own shop. Then I put the instructions and the settings on a public website where anyone can read them and copy them. Free. No signup to read. No catch.

The license on both projects is called MIT. In plain words: use it in your business, change it however you want, don't ask my permission, and I make no promises that it works for you. That last part is the "as is" clause every open-source license has. You never owe me anything. If you improve it and want to send the improvement back, [here's how](CONTRIBUTING.md), but nobody expects it.

## What GitHub is

GitHub is a website where people keep the files for a project, along with every change ever made to them. Think of it as a shared filing cabinet with a history. A "repository," which people shorten to "repo," is one drawer: one project's files. Two drawers matter here.

- **The guide you're reading:** [github.com/morriss-group/ai-for-appliance-repair](https://github.com/morriss-group/ai-for-appliance-repair). These pages are the files in that drawer, shown as a website.
- **The phone agent kit:** [github.com/morriss-group/vapi-voice-tuneup](https://github.com/morriss-group/vapi-voice-tuneup). The settings, the how-to, and every fix.

Reading needs no account. A free account matters for two things only: getting an email when I fix something, and telling me something is wrong.

## How the whole thing fits together

1. **Chapter 1** is the chat program on your desk, the one you type to. It runs nothing by itself.
2. **Chapter 2** is the phone agent. Several separate companies bill you directly, and the kit's START-HERE lists every meter under "What it costs": the voice service (VAPI) that runs the agent, with the model and the voice bundled into its minute; the phone company (Twilio) that owns the number; the hosting for the small server, once you want the agent looking at a calendar; and two optional ones behind those. The kit holds my settings and the rules I've learned to put in the agent's instructions.
3. **The booking piece** is a small program inside the kit, in the folder called tools-server, that lets the phone agent look at your calendar and put appointments on it. It has to run somewhere on the internet. This is the one part where "hand it to your tech person" is a fair answer, and the kit says so.
4. **Chapters 3 through 7** are the rest of the site. The chapter list on the front page says what each one covers.

Nothing you build sends anything to me. I can't see your setup, your calls, or your customers, and I don't want to.

## How updates work, which nobody tells you

Nothing updates by itself. When a real call shows me something wrong, I fix my agent, then I post the fix. Your copy does not change. Two things follow from that.

- Every fix is listed in the kit's CHANGELOG file, newest first, with the exact line to change in your own instructions.
- GitHub can email you each time I post one, but only if you tell it to. That's section B below.

## What to click, step by step, on a phone

### A. Make a free GitHub account

Only needed for sections B and E. Two minutes.

1. Open [github.com](https://github.com) in your phone's browser.
2. Tap the three-line menu at the top left, then "Sign up." On some phones the "Sign up" button sits at the top right instead.
3. Type your email, make a password, pick a username. Tap Continue through the screens.
4. GitHub emails you a code. Type it in. Done.

### B. Get an email whenever I post a fix

1. Open [github.com/morriss-group/vapi-voice-tuneup](https://github.com/morriss-group/vapi-voice-tuneup) and sign in. You have to be signed in for the next step; signed out, the button isn't there.
2. Near the top, under the project name, tap the button with the eye on it that says "Watch." On some phones it's tucked behind the three dots at the top right; tap those and "Watch" is in the list.
3. A menu opens with four choices: "Participating and @mentions," "All Activity," "Ignore," and "Custom." Tap "Custom."
4. Check the box next to "Releases." Leave the others unchecked. Tap "Apply."
5. From then on, each fix arrives as an email from GitHub. Open it, read what changed, and change the same line in yours.

### C. Read what changed

1. On the kit's page, scroll down to the list of files and tap "CHANGELOG.md."
2. Newest is at the top. Each item is one change and the exact wording to add to your own instructions.

### D. Get the files, only if you're building it yourself

1. On the kit's page, tap the "Code" button. It's green on a computer; on a phone it may be plain.
2. Tap "Download ZIP." Your phone or computer saves one file. On a computer, double-click it to unpack.
3. A ZIP never updates. When a fix is posted, download it again or change the line by hand from the CHANGELOG.

If your tech person uses git, they can "clone" it instead and pull updates in. They know what that means, and the kit's deploy guide says how.

### E. Tell me something is wrong

1. On the kit's page, tap "Issues," at the top next to "Code."
2. Tap "New issue." Sign in if it asks.
3. Title: what broke, in one line. Below it: what you did, what you expected, what happened. No customer names or phone numbers. It's public.
4. Tap the green button to post it. I read every one.

Or reply in the group where you found this link and say the same thing. That works too.

## Four words you'll meet, in plain English

- **API:** a way for one program to talk to another without a person clicking. When the phone agent checks your calendar, it uses your scheduling software's API. Some vendors charge extra for that door.
- **Webhook:** the reverse: a program calling you. When a call ends, the voice service sends a report to an address you give it. That is all the "webhook walkthrough" sets up.
- **Terminal:** the black window on a computer where you type commands instead of clicking. A phone doesn't have one. Every step that says "type this" happens there.
- **Agent:** a program that uses an AI model to do a job on its own: answer the phone, read a calendar, write a ticket. Nothing mystical; a very fast clerk with a script.

## What this costs

Reading and copying: nothing. Running it: the voice service, the phone number, and the model each bill you on their own. Chapter 2 and the kit's START-HERE page give the honest numbers, and they change, so I don't repeat them here.
