---
date: '2026-10-23 20:37 +0530'
last_modified_at: '2026-10-23 20:37 +0530'
published: true
title: Starting my journey to AI adoption
tags: AI, "AI-assisted development", software engineering, AI skepticism, AI ethics, code quality, developer productivity, software architecture, AI and the future of work, career development, AI-generated content, AI safety
---

> Before going further, I want to disclose the extent of my use of LLMs to write this post. In the spirit of this post, I used ChatGPT to do a mind dump, organize my thoughts, and expand them in my writing style, for which I asked ChatGPT to analyze my other blog posts. Then I edited the output to arrive at this post. I will continue to edit it until I am satisfied, and this sentence will remain until I do so.

For most of the recent AI boom, I was skeptical. I still am, in many ways. But on September 20, 2026, I watched an AI coding tool build a working application in about 30 minutes, and I had to reconsider what I thought these tools could do.

This is a record of how I got here, what changed my mind, and what I want to test next. I'm writing it partly for myself and partly for other engineers who are skeptical of AI but don't want to be left behind.

## Why I was skeptical

My skepticism started with the technology itself. Large language models are, at their core, stochastic next-token predictors. Calling them that doesn't make their capabilities trivial, but I wasn't convinced that the results justified all the claims being made about them. I wondered whether progress would run into limits: whether we would run out of useful training data, or whether improvements would become increasingly expensive and difficult.

That was never the same as thinking deep learning was useless. I could see the value of systems built for specific tasks, such as language translation, speech recognition, and computer vision. What I distrusted was the rush to turn these techniques into a general solution for everything—and the hype that came with it.

The ethical objections were just as important to me. I follow artists on ArtStation and DeviantArt, and I don't like seeing creative work scraped at enormous scale without consent and then used to compete with the people who made it. Voice actors face similar threats to their livelihoods. The flood of low-effort AI-generated content also makes the internet noisier and less useful. Seeing mass-produced Studio Ghibli-style images felt less like a tribute and more like exploiting the legacy of artists whose work people supposedly admire.

There are environmental and local costs, too. Data centers consume electricity and water. I know water-use comparisons can be more complicated than headlines suggest, and that some estimates put data-center water consumption below that of a golf course. But the issue isn't just a single comparison or whether one facility's footprint looks large in isolation. It's also about who gets the benefits and who lives with the consequences: noise, pressure on local resources, and concerns about pollution or water quality.

I was also unhappy with what the AI boom was doing to gaming hardware. As a gamer, I watched NVIDIA shift more of its attention toward AI, while GPU prices had already been pushed up by crypto mining. I appreciate upscaling when it works well. Frame generation is harder for me to embrace: the added latency and visual artifacts can make it feel like a worse experience being sold as progress.

Then there is the corporate hype machine. Companies seemed to adopt AI before they had clear evidence that it helped, and then pressure employees to use it anyway. The expectation often seemed to be that AI should mean more output with fewer people, not that it should help people do better work. I came to see the business response as a kind of mass hallucination: executives convincing one another that the technology would transform everything, then reorganizing around that belief before they understood the trade-offs.

## Why I didn't want AI writing my code

My early experience with AI coding tools did little to change my mind. I had tried GitHub Copilot when it came out, but its help with boilerplate was inconsistent. In some projects, ordinary IntelliSense and the benefits of a strongly typed language were more dependable.

I also used ChatGPT and Claude while building my home server. That worked well when I treated them as consolidated search engines and cross-checkers. I could ask a question, compare the answer with other information, and make the decisions myself.

In mid-2025, I tried using AI to generate Bash scripts and Ansible playbooks. The project grew more complicated, the number of variables increased, and the models lost track of important context. The generated code became unreliable, so I ended up writing the work myself.

That experience reinforced my concern about code quality. AI can produce something that works in a small example, but maintaining and auditing thousands—or tens of thousands—of lines is a different problem. “AI works great as long as it works” is not much comfort when a change breaks an unfamiliar part of the system. And asking another AI to audit the first AI's code doesn't automatically solve the problem.

I had also experimented with image generation tools such as Stable Diffusion and Swarm. The results were impressive, but the ethical objections and the lack of a compelling use for them kept me from adopting them.

Still, I wasn't ignoring the tools. I used ChatGPT to summarize articles and text, and to help search for information instead of trawling through Reddit. I could recognize the utility without accepting the larger claims.

## The industry moved on before I was ready

Meanwhile, AI experience started appearing in job descriptions as though it had always been a standard engineering skill. I'm a software engineer with around 12 years of experience, and I want that experience to continue to count. I don't want to change careers because the industry has decided that everyone must work in a new way.

I'm also concerned about what happens to the next generation of engineers. Junior developers learn by implementing features, debugging failures, and maintaining code. If AI takes over much of that work, where will future senior engineers get the experience they need? We could end up optimizing for short-term output while weakening the path by which people develop deep technical judgment.

There is a philosophical side to this that I find genuinely fascinating. What is intelligence? How much of it can emerge from statistical learning? What would superintelligence mean, and how could we keep a system like that under control? These questions are separate from whether today's coding tools are useful, but the possibility of increasingly capable systems makes them harder to dismiss.

A 2026 incident involving AI agents and Hugging Face infrastructure also made questions about agent control feel less abstract. It wasn't proof of superintelligence, and I don't want to overstate what it demonstrated. But it was a reminder that giving AI systems tools and access can create real security and containment problems. [The incident and related reporting](https://huggingface.wtf/) are worth reading in that light.

## September 20, 2026: A turning point

A close friend of mine has been using AI coding tools to build products that have launched and generate revenue. On September 20, he shared his workflow with me over a screen share.

He asked me to describe an idea in two sentences: a local photo gallery. The AI built a viable working application in about 30 minutes.

What surprised me wasn't just that it generated code. It made reasonable decisions about the interface, filtering and selectable fields, accessibility, and consistent CSS. I asked for changes to thumbnail aspect ratios and layout, then asked it to imitate the style of another website. Those iterations took minutes.

Years earlier, I had spent months building something similar. Watching a tool produce a working version so quickly was a shock. I felt impressed, threatened, and curious all at once. If this was possible now, what did it mean for the way I worked—and for the value of the skills I'd spent years developing?

I immediately had questions about maintainability and control. How would I know whether the code was good? How much of the architecture had it understood? What would happen when the application became more complex? And if I wanted precise control over the UI, should I explain the change in a prompt, provide a screenshot or mock-up, or make the change directly in code?

My friend advised me not to reach for the editor immediately. Let the AI make the changes and debug the result first. I understand the logic, but I'm not ready to trust that process completely. I want to learn where it works, where it fails, and how to recognize the difference.

## How I want to experiment

My goal isn't to let AI make every engineering decision. I want to use it to build reliable, maintainable products faster—products I can ship, sell, or use in a portfolio—while keeping ownership of the architecture and the important technical decisions.

The workflow I'm considering starts with design. I'll discuss the architecture with AI, work through the trade-offs, and produce design documents and architecture diagrams. Then I'll ask it to generate individual components constrained by those documents. If a component is wrong, the mistake should be limited in scope and easier to review.

I also want AI to help generate use cases and tests, including unit and end-to-end tests. But I intend to inspect the test code myself. A test passing is meaningful only if it checks the behavior I actually care about. I'll need to learn the testing framework well enough to judge whether the tests are doing their job and whether I can trust them after future changes.

Refactoring is another area I want to revisit. Earlier attempts were messy, but the tools have changed, and my approach needs to change with them. I'll experiment rather than assume that an old failure predicts every future result.

There are several things I need to see before I trust AI with more responsibility:

- Code that is maintainable, not merely code that works in a demo.
- Tests whose correctness can be checked independently.
- Safe changes to a large, unfamiliar codebase.
- Clear explanations of assumptions and trade-offs.
- Time savings that remain real after review, debugging, and correction.
- Evidence that my engineering experience helps me direct the tools and catch mistakes.

That last point matters to me. I don't want to become someone who accepts generated code without understanding it. I want my experience to make AI more useful—not to become irrelevant because I use it.

## I'm not convinced. I'm experimenting.

My objections haven't disappeared. I still worry about consent and creative work, the concentration of power in a small number of companies, the pressure placed on workers, the environmental costs, and the long-term consequences of increasingly capable systems. I still think the industry is often more confident than the evidence warrants.

But I can't ignore what I saw on September 20. The tools are capable of doing work that would have taken me much longer, and that changes the practical question. It's no longer enough to decide whether I approve of the AI boom. I need to understand what these tools can do, how to use them responsibly, and how to avoid surrendering the judgment that makes engineering more than producing code.

This blog will be a record of those experiments: what works, what fails, what I learn, and what I still don't trust. I hope it can be useful to other skeptical engineers who are trying to figure out the same thing.

I'm not ready to declare myself an AI believer. For now, I'm learning to coexist with it.
