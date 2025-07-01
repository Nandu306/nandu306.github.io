---
layout: post
title: "From Apps to Agents: How AI is Becoming Personal"
description: How I built an AI agent for German learning and what it signals about the future of personalised software
date: May 2025
image: /public/teaching.jpg
---

If 2024 was about AI chat interfaces, 2025 is all about AI agents - digital elves that actually do some heavy-lifting on your behalf, personalised to your whims and fantasies, without your intervention. This could be anything from planning and booking a holiday to managing your social media presence or updating your CRM system with a new blog post.

But the implications go far beyond personal productivity - we're talking about AI agents that could replace entire job functions, from research analysts to executive assistants.

### The AI Agent Product:

In the spirit of exploring, especially as there now seems to be plenty of no-code AI automation options, I built a tool that addresses a personal pain-point: finding and reading German content at my right proficiency level. Having now finished with formal classes (I spent the past 8 months learning German in an evening class), it has been challenging to expose myself on a recurring basis to the language, especially as my day-to-day life doesn't revolve around German. Whilst <a href="https://www.nachrichtenleicht.de/" target="_blank">Nachrichtenleicht</a> is an option, I wanted something more personalised with some grammar pointers thrown in. I also wanted something that would be sent to me so that I don't leave things to chance. 

Although there are quite a few no-code tools to choose from (<a href="https://www.make.com/en" target="_blank">Make</a>, <a href="https://n8n.io/" target="_blank">n8n</a>, <a href="https://www.lindy.ai/">Lindy</a>, <a href="https://zapier.com/">Zapier</a>), I chose <a href="https://www.relay.app/" target="_blank">Relay.app</a> for its intuitive design, simplified workflow setup and the amount of resources available online. The workflow (as shown in the screenshot below) is straightforward: the agent is triggered every day at 8am; it checks the RSS feed of Die Zeit (a leading German news provider); an AI model then rewrites the news item to my B2 proficiency level, including vocabulary and grammar explanations in English; and finally, an email is sent to me.

[![Photo of an AI agent workflow on Relay.app](/public/ai_workflow.png)](/public/ai_workflow.png)

For those interested in the prompt mechanics, I have included the prompt as well. I opted to use Gemini's 2.5 Flash as it is generally known to be good at language-related tasks (Relay.app gives the option to choose your model).

> Pick 3 current news items and rewrite them so they are accessible to someone working towards a B2 CEFR level in German.
>
> **Rewriting Guidelines:**
>
> * Length: Each news item should be 4-6 sentences (60-100 words) to provide sufficient context and detail.
> * Use simple sentence structures while maintaining key information.
> * Limit sentences to 15-20 words maximum.
> * Replace complex vocabulary with B2-appropriate alternatives.
> * Maintain factual accuracy while simplifying language.
> * Include essential details: **who, what, when, where,** and basic **why/how.**
>
> **Vocabulary Highlighting:**
>
> Highlight words that are:
>
> * Above A2 level but essential for B2 comprehension.
> * Key nouns, verbs, and adjectives central to understanding the news.
> * Words with multiple meanings or specific contextual usage.
>
> **Grammar Explanations:**
>
> Focus explanations on:
>
> * Grammar points that appear in your rewritten text.
> * Common B2-level challenges (cases, verb positions, subordinate clauses).
> * Maximum 2-3 grammar points per news item to avoid overwhelming learners.
> Write all grammar explanations in English for better comprehension.
>
> **Example:**
>
> Nachricht 1: Manager in der Türkei
> In der Türkei **stehen** einige wichtige Manager **vor Gericht**. Sie hatten Präsident Erdoğan **kritisiert**. Aber jetzt, in der **Krise**, braucht Erdoğan ihre Hilfe.
>
> **Vokabeln:**
>
> * **stehen** (steht, stand, gestanden) – to stand; (here) to be (e.g., before a court)
> * **vor Gericht** – before court / on trial
> * **der Präsident** (die Präsidenten) – the president
> * **die Krise** (die Krisen) – the crisis
>
> **Grammatik-Erklärung:**
>
> * **Verb Position in Main Clauses:** In a German main clause, the conjugated verb (in this case, *stehen* - to stand/to be) always occupies the second position. For example: "In der Türkei stehen Manager vor Gericht." (In Turkey, managers are on trial.)
> * **Dative with the Preposition "vor":** The preposition "vor" (before/in front of) can take either the dative or accusative case. When used with "vor Gericht" (before court), it expresses a location or state, which is why the dative case is used (das Gericht becomes dem Gericht). If "vor" were used with the accusative case, it would express movement.

### The Bigger Picture:

Building this individual AI agent is an indication of how future SaaS platforms might evolve: hyper-personalised and built by the consumer themselves. There are several implications to this. On one hand, I'd imagine that the one-size-fits-all solution embraced by most enterprise solutions might be disrupted as consumers can now themselves craft and build solutions that are tailored for their use cases. This also means that consumers should be more tech-savvy, explore options that enable them to build tools on their own and generally embrace a more product mindset.

On the other hand, AI agents can transform how societies function. There is talk of hyper-personalised learning rather than fixed curricula in schools and solo entrepreneurs running million-dollar businesses with AI agents handling customer support, content creation, and daily operations while they focus on strategy and growth.

Whether these materialise in the short-term or not, we cannot deny that AI automation is going to have a real impact on how we get things done. So, food for thought: What would you build an AI agent to do for you?
