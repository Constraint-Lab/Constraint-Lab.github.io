---
title: How AI changes our system of work
tags: ai
---

> So your company is making thirty-six percent more money from your plant just from installing some robots? Incredible. - Jonah from _The Goal_

AI is impressive technology, but more interesting to me is how we apply the technology. The fast rollout has some good and some bad. In my experience, no one has done a sufficient job of explaining the rules on determining what's good and what's bad. And I'm not talking about experience reports, vague mandates, or arguments that hand-wave the important details.

It seems obvious to me that our current plan of tokenmaxxing is not just bad from a Goodhart's Law perspective. It's also bad because simply maxing out running of LLMs doesn't help even if everyone was fully bought into the mission.

Eli Goldratt's four questions of new tech seem like the way to get the rules I'm looking for.

1. What is the power of the new technology?
2. What limitations does the new technology diminish?
3. What rules helped us bypass the limitation?
4. What are the new rules?

## What is the power of AI?

There are a few different ways I'd describe it, depending on how abstract I need to be:

1. AI is good at cheaply generating plausible hypotheses.
2. AI is good at cheaply testing hypotheses.
3. AI is good at taking loosely structured data and transforming it into differently structured data.

The connection is, the transformation in step 2 is not guaranteed correct. It has to be validated against reality. That process is just a small, scientific experiment. Therefore, the output of the transformation is an hypothesis.

AI is very good at generating a reasonable hypothesis, testing it against whatever reality it can access, and then creating a new hypothesis based on the results.

Put succinctly: AI can, by the process of generating and testing hypotheses, cheaply answer any question with a hypothesis that has a ~good chance of being proven correct. (It's a bit like Jeopardy where every answer to the question must be a question. Any statement can be easily transformed into a question, it just takes a bit to get used to thinking about that way.)

## What is the limitation AI diminishes?

All software is a hypothesis: "I predict that this set of instructions will result in this behavior." If you tried to randomly generate instruction sets, you'd be surprised if you could even get something that had the proper syntax, let alone behavior. Every plausible set of instructions required human effort and understanding.

Restated in our AI language, generating a reasonable hypothesis is expensive because it requires human effort and understanding. Validating a hypothesis is expensive because it is potentially risky and requires human effort and understanding. Depending on the context, AI has made those statements mostly false or completely false.

## What rules helped us bypass the limitation?

#### 1. We route work to get the most efficient use of human effort.

Take code reviews. If it's a simple, safe change, ~anyone can sign off. If it's risky or complex, get a principal involved. Don't submit half completed code for review, unless there's a specific reason you need help at that point. Prefer reviews from someone who has context, so we don't require the extra human effort of gaining context.

#### 2. We use linters.

Here go a bunch of rules to amortize the cost of human effort that goes into deciding things like coding style. Let's answer this question once so we never have to spend human effort on it again. Let's make it automatic so no one ever has to think about it again.

#### 3. We have upfront design.

It's expensive to build the wrong thing. The further a design gets into production, the more human effort required to pull it back.

#### 4. We reject upfront design.

It's expensive to design a bunch of things on paper that don't translate to code and/or end up never getting built.

#### 5. We use automated testing, canaries, and phased rollouts.

We're not sure our code is correct, so we verify it against reality. How we verify is determined by cost and value. Unit tests are low on the cost scale but also low on the value scale. Production is the opposite.

#### 6. Risk separated code

Config changes require approvals from multiple principals. A typo on the careers page gets a "LGTM". Credit card processing is a completely separate org with access strictly gated.

This isn't an exhaustive list of rules nor does it explain every reason the rule exists (e.g. code reviews share accountability). It does show how reducing human effort, specifically of the "human thinking" variety, along with risk management, underlines so much of our system of work.

### Analyze the rules

Before figuring out the new rules, we should see that our old rules are built on an important assumption. Because every reasonable hypothesis required human effort/understanding, you could assume human understanding + reasonable hypothesis always traveled together. It was safe to use "this is reasonable" interchangeably with "some human understands this."

*That assumption is **totally broken**. It is not true anymore at all.*

Code review approval? Could be Alice, could be Claude.

PR that passes all the tests? Could be Bob, could be Codex.

Ten page design doc? Definitely an LLM.

Code reviews assumed there was a human on the other side we could jump on a call with and explain how it works. We assumed that the twenty commits going out in the next release were backed by ~20 people who understood each commit. It was safe for all of our rules to assume this, so every rule potentially needs to be changed. This assumption was load-bearing (a human person typed that, relax, it's just a cheap joke).

## What are the new rules?

Answering this is a lot of work. The new rules aren't determined by blindly negating the old rules. Getting rid of code reviews and just shoving all the commits on main _might_ work, but other parts of the system would need to change. And code reviews are not just about ensuring correctness, they're also about security/accountability. So if we get rid of code reviews, we need to satisfy all of the reasons that rule was there. We're changing a system of work, so any local changes have to be weighed against their impact on the entire system.

As I mentioned, it's a lot of work, so that will be the work of the next post.
