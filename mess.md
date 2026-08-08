I know I promised this would be about the new rules, but we need to talk more about the now invalid assumption we've all been carrying. One, we need to fully internalize how baked in that assumption is. Two, we need to see why a naive deployment of AI is soul crushing if we don't recognize that assumption. And last, we need a clear picture of the problem before we discuss the new rules.

To restate the assumption AI has now made invalid: *valid artifacts are no longer proof of human understanding.*

## Understanding as a limiter

Understanding is a prerequisite for reliability. The reliability required determines the appropriate amount of understanding. This means that we've always been required to understand our systems. Our assumption meant no one had to say this or test for this (we'll come back to this).

Each individual's work required understanding, so we had natural throttles throughout the system. The number of PRs I could create wouldn't be 10x yours, so even though you often had to choose between writing and reviewing code (notice this stress was already in the system), it was manageable.

When we each took our on-call shifts, we had either written or read much of the code we were responsible for. In other words, we understood the code we were responsible for. And when we did run into something we didn't understand, we always had escalation paths to someone who did.

## AI as a 10x'er

So now I get access to AI, and it's just in time because I have an insane deadline. I take just a bit of a shortcut and use AI to write some of the code. I read it, it mostly makes sense, passes all the tests, etc. I've just doubled the number of PRs you have to review.

How do you handle it? Do you work more hours? Write less code and miss your deadlines? Work at the same rate and block my work? Or do you accept the mandate to use more tokens and have AI help you just a bit?

Once you give in to the pressures of the system, you start using AI just a bit more and your system understanding starts slipping just a bit. And now the cycle as begun.

This to me is the spiral that is quickly getting out of control. We use more AI, and our understanding slips a bit. Then we understand less, so we rely more on AI. We rely more on AI, so our understanding slips even more. The entire time, more and more PRs are flowing through the system. And as this happens, we feel the stress of being responsible for a growing system that we understand less.

And this is pressure from our system of work. Even if you have iron-will discipline to always fully read and understand every bit of code and every decision, you're exercising that discipline every moment of every day. You also have way more code to review. So even the best, most responsible engineers aren't immune. As Deming said, "A bad system will beat a good person every time." 

To summarize: we're busier than ever, doing less of the work we enjoy, while being more stressed about system stability, inside of a system that enforces each of those.

## Attempted solutions

As best as I can tell, all solutions revolve around the premise that we don't need to understand the code. Unfortunately, I've not seen risk be adequately acknowledged with these solutions.

If ~0 people care if you cause an incident, you don't really need to understand your code. And if you're in a start-up survival situation where you're not sure you'll even be here next month, then better to ship something you don't understand today and hope you're around tomorrow to figure it out. In many cases, there is no relevant risk to not understanding your code.

In many cases, especially the ones I get paid for, none of that is true. The code I write is expected to run for years. Others will build on it. If it fails, lots of people definitely care. I don't see harnesses or test suites or whatever as being replacements to understanding the code.

Let's say we have an incident. I see four options:

1. An LLM fixes it
2. An engineer understands the system and fixes it
3. An engineer doesn't understand the system, so they first gain understanding and then fix it
4. Sorry boss, that just stays broken

Option 1 is great, and we should use that as much as possible. But, that's not always possible, and in those cases, option 2 is greatly preferable to 3 and 4. So when we use option 1, we need to consider if it conflicts with option 2 when we need it, along with the expected cost of options 3 and 4.

You can't undermine option 2 unless you're willing to pay the costs of options 3 and 4. And because LLMs will generate whatever they want that satisfies the verifications we put in place, verifications which themselves were not sufficient to stop the incident, we can't assume that understanding the verifications/intents/whatever is sufficient to understand the running system. (We also shouldn't ignore that each option has a different probability of causing more incidents.)

All that to say, I'm not convinced that a combo of good testing and code review maintains the required understanding of our systems. 

Unless I miss my mark, we're on our way to a steady state of misery until we change the design of our system of work.
