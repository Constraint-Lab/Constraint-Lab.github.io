---
title: AI is a bubble, just like dot-com
tags: ai
---

<blockquote class="twitter-tweet"><a href="https://twitter.com/bostonou/status/2085097056159318275">August 5, 2026</a></blockquote>

<p class="post-disclaimer">I tested out having Claude generate the final draft. Results were quite clear that people would not read it lol.</p>

Andrej Karpathy has written large language models the way most of us have written CRUD apps. He was a founding member of OpenAI, ran AI at Tesla, and joined Anthropic this spring to train Claude. He wrote nanoGPT and llm.c, the small readable codebases people use to learn how a language model works end to end.

When Anthropic put Claude inside Slack, he called it ["a new paradigm"](https://x.com/karpathy/status/2069547676849557725) — the third major redesign of how humans use these systems. Not a website you visit anymore, not an app you install, but "a self-contained, persistent, asynchronous entity with org-wide tools and context, working alongside teams of humans."

He closed with: "it works and it is awesome."

The replies had a different read. One of them, in full:

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">&gt; This is a new paradigm<br><br>brother it&#39;s a slack integration<br><br>I miss the old andrej</p>&mdash; @MatthewFoxAF <a href="https://twitter.com/MatthewFoxAF/status/2069709303234146384">June 24, 2026</a></blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

Hold that exchange still for a second. Nobody in it is stupid. That's what makes it worth understanding.

The same split runs through everything right now, and nothing around it holds still.

Leadership says "use more AI," and never defines responsible use. Engineers hear it through an older instinct: don't ship what you don't understand. Nobody explains how both survive.

Layoff announcements credit AI in the same breath as the earnings beat. A colder fear sits underneath: people who own the AI on one side, people whose work it does on the other, no visible way across.

The ground keeps moving. Prompt engineering was a job title. OpenClaw picked up a hundred thousand GitHub stars and caused a Mac Mini shortage in the same week. Ralph was the future for about a weekend. Context engineering, then harness engineering, then graph engineering. Each was the obvious way to work, right up until the next one was. The gaps keep getting shorter.

And everywhere, teams ship code faster than they can understand it. Ask whoever's on call.

I'd love to stand cleanly on one side of all this. I can't. I haven't written a line of code in about a year. Claude writes it all. These posts too. I read all the code before it ships, and I still feel the difference. Understanding used to be a byproduct of writing the code myself. Now understanding is a separate job.

Both perspectives, one person.

There's a default way to resolve contradictions like these: decide who's deluded. "I miss the old andrej" does it in five words: if Karpathy calls a Slack bot a paradigm, something must have happened to Karpathy. Sorting people into right and wrong passes for rigor. It assumes that when two perspectives contradict, one of them must be false.

Our industry tested that assumption once before, at scale.

In March 2000 the NASDAQ peaked above 5,000. By October 2002 it had lost 78 percent of its value. Pets.com IPO'd in February and was gone by November. The sock puppet outlived the company. Betting against it was exactly right.

Amazon lost more than 90 percent of its stock price in the same crash and kept shipping. Within a decade the internet had rearranged retail, news, music, and how you found a job. Betting on Amazon was exactly right too.

Same year. Same technology. "Wildly overhyped" and "changes everything" were both correct at the extreme.

Nobody had to be deluded.

And there were four ways to stand, not two. Short everything: it's all a bubble. Long everything: it's all the future. Long Pets.com, short Amazon: backwards twice. Long Amazon, short Pets.com: right twice. The first two are moods about a technology. The last two are judgments about cases. The only thing separating right twice from backwards twice was understanding.

None of it was magic. The information separating a Pets.com from an Amazon was public the whole time. The hard part was knowing what question to ask of it. What could the internet do that nothing before it could? A bookstore with every book in print, yes. Free shipping on forty-pound bags of dog food, no. Most people, watching the same screens, never asked. They picked a mood and waited for the grade.

We're inside the next one now. That may be the only point the amazed and the unimpressed already agree on: whatever this is, it's big.

Transformational technology comes along maybe twice in a working life. I was in school for the last one, watching different screens: South Park, Perfect Dark, Conker's Bad Fur Day. This time I want to understand it while it's moving: test hypotheses against what happens, and decide how I work while the decision still matters.

You're inside it too. Your feed has already assigned you a position: be amazed, or be afraid. Both are moods. Understanding isn't assigned. You have to go get it.

So start where understanding starts. What is the disagreement about?

Mostly not models. There are arguments over which model is best, and over whether open weights beat closed ones. They stay small and almost polite. The real fights are somewhere else. Do you read every line the model writes? Can you ship code you don't understand? Do passing tests mean it works? Does an AI review count as a review? Every team I know is re-deciding these rules on the fly. Some decide with conviction. More sound like: we don't know what to do, but we'd better do something.

Model quality enters at one point only: "the models will get so good that none of this will matter."

Maybe.

So here's my first hypothesis, stated so you can hold me to it. Models will not become dependable enough, soon enough, to settle these questions for us. If you're sure that's wrong, sure that near-flawless output arrives in a year or two, you can stop reading. The questions will answer themselves, and this series with them. I don't think that's where we are.

Now set the pieces next to each other. Intelligent people look at one technology and see wildly different things. History says conclusions that far apart can both be correct. And the rule debates run on, team after team, without resolving. Arguments that run this long between capable people are built on assumptions nobody has checked. We've already seen one: somebody has to be wrong. The rule debates lean on another that nobody has said out loud. Behind that one is the question that sorted Amazon from Pets.com, aimed at our own work this time.

What did this enable that we couldn't do before?

Each of those rule debates assumes an answer to it. That's the question this series works out. One small, checkable step at a time. I'm writing to answer it for myself. You're welcome to come along and check the work. By the end you won't need my conclusions. You'll have your own read on any AI claim that crosses your feed.

Including this one: AI is a bubble, just like dot-com.

---

*Thanks to [Emma Bukacek](https://www.linkedin.com/in/emma-bukacek-%F0%9F%8D%89-69822249/) and [Tim Pote](https://www.linkedin.com/in/timothypote/), who read early drafts and told me what wasn't working.*
