# PRD
Vibe coding guide

Vibe Coding Isn't Dumb - You're Just Doing It Wrong
(A practical guide for shipping apps with AI & minimal pain)

Vibe coding gets a lot of hate, especially from "serious" devs. But the truth is: not every project needs to be scalable, secure, or architected like it's going public on the stock market.

Most of the time, you just want to turn your idea into a working app - fast. Here's how to do it without driving yourself insane. These aren't fancy tricks, just things that work.

1. Pick a mainstream tech stack (zero effort, high reward)

If you're building a basic website, just use Wix, Framer, BlackBoxAI or any other site builder. You don't need to code it from scratch.

If you need a real web app:
-> Use Next.js + Supabase.

Yes, Svelte is cool, Vue is nice, but none of that matters when you're trying to get something done. Next.js wins because it has the largest user base, the most examples online, and AI is most likely to get it right. If your backend needs real logic, add Python.

If you're thinking about building a game:
-> Learn Unity or Unreal.

Trying to vibe-code a game in JavaScript is usually a dead end. Nobody's playing your Three.js experiment. Be honest about what you're building.

💡 Skip this rule and burn your days fixing the same bugs that AI could've solved in seconds - if only you'd picked the stack it knows best.

2. Write a simple PRD (medium effort, high reward)

You don't need a fancy spec doc. Just write a Product Requirement Document that does two things:

Forces you to clarify what you actually want.

Breaks the work into small, clear steps.

Think of it like hiring a contractor. If you can't write down what "done" looks like for Day 1 or Week 1, your AI won't know either.

Once you've got the plan, give the AI one step at a time. Not "do everything at once."

Example:
Chat 1:
"Implement Step 1.1: Add Feature A"
Test it. Fix it. Then:
New Chat:
"Implement Step 2: Add Feature B"

Bugs compound over time, so fixing them early saves you from a mess later.

3. Use version control (low effort, high reward)

AI will eventually break your code. Period.

You need a way to roll back. Most tools have automatic checkpoints, but it's better to use Git. Manual commits force you to actually track progress, so when AI makes a mess, you'll know exactly where to revert.

4. Provide working code samples (medium effort, high reward)

Don't assume AI will get third-party libraries or APIs right just from docs.

Before you start building a full feature, write a small working script that does the core thing (e.g., pull 10 Jira tickets). Once it works, save it, and when you start the real task, pass it back into your AI prompts as a reference.

This small step will save you from wasting hours on tiny mismatches (wrong API version, bad assumptions, messed auth headers, etc.).

5. When stuck, start a new chat with better info (low effort, high reward)

The "copy error -> paste to chat -> fix -> new error -> repeat" cycle is a trap.

When you hit this loop, stop. Open a fresh chat and tell the AI:

What's broken.

What you expected to happen.

What you've already tried.

Include logs, errors, screenshots.

The longer your chat history gets, the dumber the AI gets. A clean context and clear input often solves what endless retries can't.
