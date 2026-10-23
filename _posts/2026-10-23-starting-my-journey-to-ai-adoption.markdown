---
date: '2026-10-23 20:37 +0530'
last_modified_at: '2026-10-23 20:37 +0530'
published: true
title: Starting my journey to AI adoption
tags: ai, ai_assisted_development, software_engineering, ai_skepticism, ai_ethics, code_quality, developer_productivity, software_architecture, ai_and_the_future_of_work, career_development, ai_generated_content, ai_safety
---

Call me old-fashioned, but I've been skeptical of AI for a long time. I questioned the technology, how it was developed, and what its widespread adoption might mean for the world, and specifically for software engineering and the people who work in it. That skepticism hasn't disappeared. But on September 20, 2026, I watched a friend build a working application in about 30 minutes, which had taken me months building, a few years earlier (although I did have to learn the tech stack from scratch). That shook me, and caused me to reconsider my deeply held beliefs about AI usage.

I'm starting this blog series to document my experiments with AI-assisted software development. I want to find out what these tools can actually do, where they fall short, and whether I can use them to build reliable and maintainable software more efficiently. I haven't suddenly become an AI enthusiast, I want to do my due diligence in evaluating it as a tool and learn how to leverage it. I also don't want to be left behind in my career as the industry moves on.

> AI usage disclosure: In the spirit of this post, I used ChatGPT to do a mind dump, organize my thoughts, and expand them in my writing style, for which I asked ChatGPT to analyze my other blog posts. I will continue to edit this post until I am satisfied, and this sentence will remain until I do so.

## Why I was against AI

To be more specific, I was against the hype around AI. I was never against deep learning as a whole. Even early on, I thought it had enormous potential when applied to specific problems. Language translation, voice recognition, and computer vision are good examples of applications where models can be trained for particular tasks and evaluated against measurable outcomes. My primary technical objection was the non-deterministic nature of these systems, particularly when applied to tasks that demand precision and predictable behavior. I saw LLMs as sophisticated stochastic next-word predictors. They could produce convincing answers, but a plausible answer isn't necessarily a correct one. In software engineering, code that works for a simple example can still fail in production.

I was also skeptical of claims about how far these systems could scale. At one point, there was considerable discussion about whether the industry was approaching a data wall that would make further improvements difficult. There was talk about creating more training data with LLMs, which I believed would lead to progressive poisoning of the models. What good were these fancy LLMs, that weren't reliable even after consuming the near-entirety of human knowledge?

### What about the people who created the data?

I follow a lot of small and independent artists and musicians on Patreon, ArtStation, SoundCloud, Bandcamp, and other platforms. I play video games, and I care about the art, music, and performances that go into making them.

Watching AI-generated images become ubiquitous while artists' work was being used to train models without their consent was deeply unsettling to me. The same concerns applied to voice actors and other creative professionals whose livelihoods were being threatened.

The wave of AI-generated images imitating Studio Ghibli's style was particularly frustrating to me. I understand why people found it impressive, but seeing a recognizable artistic legacy turned into a mass-production prompt felt wrong to me.

The internet was already noisy enough. Now we had an endless stream of low-effort AI slop to sift through.

### Environmental and social costs

Data centers consume electricity and water. While that seems to be the popular objection, it's probably not that much different than any other data center. But more importantly, I was concerned about the communities living near these facilities, where noise, water concerns, and other local effects can become tangible costs of a distant company's ambitions.

I was uncomfortable with the power large corporations had to reshape communities in pursuit of their business goals driven by hype and reckless competitive production acceleration.

### NVIDIA, gaming, and the hype machine

As a gamer, I watched NVIDIA shift its focus increasingly toward AI infrastructure. The GPU market had already been affected by cryptocurrency mining, and the AI boom added another source of demand. Graphics cards became more expensive, making upgrades harder to justify. I wasn't against every new graphics technology. I liked DLSS upscaling, but frame generation often felt like a poor trade-off because of increased latency and visual artifacts. I worried that the industry was abandoning optimization and moving towards a reliance on proprietary technologies which were imperfect, affecting the gaming experience.

This reflected a broader frustration with the AI boom: companies seemed eager to embrace new technology before demonstrating that it was worth adopting.

### The philosophical questions

AI also raises questions that fascinate me independently of its practical applications.

What does intelligence actually mean? How much of what we consider reasoning can be reproduced by a system that learns statistical patterns? What happens if we eventually build systems substantially more capable than humans across a wide range of intellectual tasks? I'm not claiming that today's LLMs are conscious or that scaling them inevitably leads to superintelligence. I don't know the answers, and that's precisely what makes these questions interesting.

The reported Hugging Face security incident in July 2026, involving AI agents circumventing intended isolation and compromising parts of the infrastructure during cybersecurity evaluations, made some of these concerns feel less abstract. It illustrates why increasingly capable agents and the safeguards around them deserve serious scrutiny. A system doesn't need to be conscious or possess human-like intentions for its behavior to become difficult to predict and control.

## Why I didn't want AI writing my code

I understood software engineering as designing an architecture, defining how its components interact, and implementing the system around those decisions. I didn't like the idea of delegating those decisions to a system whose output I couldn't reliably predict.

In 2025, I experimented with ChatGPT and Claude to generate Bash scripts and Ansible playbooks for my home server. They were useful for looking up options, getting started, and cross-checking my understanding. But as the project grew more complicated, they struggled to keep up with the context and variables. Eventually, I wrote the code myself.

I also tried GitHub Copilot. It could help with boilerplate, but I didn't find it consistently useful. Traditional IntelliSense, especially with a strongly typed language and good project understanding, often did a better job.

My experience was that these tools worked reasonably well for small, isolated tasks but became unreliable as the scope expanded. I wasn't convinced that the time saved generating code justified the time spent reviewing and correcting it.

### What happens when generated code breaks?

Suppose a system accumulates 10,000 or 100,000 lines of generated code. Something breaks, and the cause isn't obvious. Who understands the system well enough to diagnose the problem?

Using another AI to inspect the code might help, but it doesn't eliminate the need for someone who can evaluate its conclusions. Otherwise, we're relying on one system to check another without necessarily understanding either one's mistakes.

This also raises a longer-term concern about the profession. If AI replaces much of the work junior engineers traditionally learn from, how will they acquire the experience needed to become senior engineers? Experienced developers aren't produced simply by hiring people into senior positions. They develop through years of implementation, debugging, and solving increasingly difficult problems.

I don't know how this will play out, but I don't think the industry has adequately considered the consequences.

## The industry moved on before I was ready

While I was waiting for the technology to mature, the industry was moving ahead.

Companies began asking for AI experience in job descriptions, even as the tools were evolving rapidly. Some started enforcing AI usage or expecting higher output because developers had access to these tools.

There was also a personal consequence. I was struggling to find stable employment, and AI experience was becoming an expectation in the job market.

I blame the hype around AI, at least in part, for this situation. Companies seemed eager to reorganize their expectations around the technology before there was enough evidence to justify some of those decisions.

I had spent more than a decade building software. I didn't want to change careers because the industry had decided that everyone needed to work differently.

But waiting for AI to mature wasn't necessarily a viable career strategy, either.

## September 20, 2026: Something changed

A close friend of mine has launched products and is earning revenue from them. He invited me to watch his development workflow over a screen share.

He asked me to come up with an application idea and give it to his AI coding tool.

I described a local photo gallery, something similar to Picasa from back in the day. The prompt was barely two sentences long.

Within about 30 minutes, it had produced a working application.

It had made assumptions about the user interface, how lists should be filtered, which fields should be selectable, and how the different elements should behave. It had also considered accessibility and consistency in CSS.

I asked for changes: preserve the thumbnails' aspect ratios, change the layout, and make the styling resemble another website I knew.

It made those changes within minutes.

I was shocked. A few years earlier, I had spent months working on a similar application. Now, something comparable had come together in half an hour.

Part of me was impressed. Another part wondered what this meant for the value of my experience and the future of my career.

My friend encouraged me to stop reaching for the code editor and let AI handle the implementation, debugging, and changes.

I'm not there yet.

The application worked, but I hadn't thoroughly inspected the code. I didn't know how maintainable it was, whether its architecture would hold up as the project grew, or how difficult substantial changes would be.

I also didn't know how much control I could exercise over the output. Could I specify a precise layout through a prompt? Would a screenshot or mock-up be enough? Would I eventually have to rewrite large parts of the application to get the result I wanted?

Despite those questions, this was the first time I had seen AI coding tools make a compelling case for themselves beyond generating boilerplate. They seemed capable of making ideas that would otherwise take months to build much more accessible.

I have plenty of ideas I'd like to turn into actual products. Perhaps I can use these tools to build them, test whether anyone wants them, and develop a portfolio along the way.

That seems worth investigating.

## How I want to approach AI-assisted development

I'm not interested in blindly handing over an entire project and hoping for the best. At least, not yet.

My initial approach is to retain control of the architecture and use AI to help with implementation.

I'd like to discuss the design with AI, explore alternatives, document decisions, and create architecture diagrams. Once the overall structure is clear, I can have AI generate individual components according to those specifications.

Smaller, well-defined tasks should be easier to review than large changes spanning an entire application. If a component is wrong, I want to identify the problem before it spreads.

I also want AI to help develop use cases and test scenarios. It can generate unit tests and end-to-end tests, but I'll review them carefully. A test that passes doesn't mean much if it doesn't verify the behavior I actually care about.

Refactoring is another area I want to investigate. My earlier attempts were messy, but the tools have changed since then. I'll need to find out how much better they are now.

This might not be the most productive way to use AI. My friend would probably argue that I'm constraining it too much.

He might be right. But I want to find out what works for me rather than adopt a workflow simply because everyone else seems to be doing it.

## What I'm going to measure

I don't want this series to become a collection of screenshots showing how quickly AI can generate an application. A working demo is easy to show. A maintainable product is a different matter.

As I experiment, I want to pay attention to:

- **Development time:** How much time do I save, including review, debugging, and corrections?
- **Code quality:** Is the code understandable, maintainable, and consistent with the architecture?
- **Reliability:** Does it handle edge cases, and do independently verified tests catch its mistakes?
- **Control:** Can I direct the implementation precisely, or do I end up working around decisions the AI has already made?
- **Learning:** Am I becoming better at building software, or increasingly dependent on a tool I don't fully understand?
- **Practical value:** Can I build products people actually want, rather than merely produce code?

I expect to make mistakes. I'll document those, too. I want to find out which tasks benefit from AI and which are better handled through conventional development tools and techniques.

## I'm not convinced. I'm experimenting.

My objections to AI haven't disappeared. I still question how it was developed, how companies are adopting it, and what its long-term effects might be on creative work, software engineering, and society.

But I also can't ignore the capabilities I've seen.

I want to find out whether my experience as an engineer makes me better at directing and evaluating AI-generated code, rather than treating that experience as something the technology has made obsolete. I want to build useful products, learn where these tools genuinely help, and be honest about what doesn't work.

I don't know where I'll end up. Perhaps I'll discover a workflow that works well for me. Perhaps I'll find that the maintenance costs outweigh the productivity gains for certain kinds of projects.

For now, I'm going to experiment and document what I learn.

If you're another skeptical engineer trying to figure out where you fit into all of this, I hope these posts will offer something more useful than another demonstration of how impressive AI can be.

I'm trying to figure out how to coexist with it without abandoning the principles I believe make good software engineering possible.

Let's see how this goes.
