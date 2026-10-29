---
name: human-friendly
description: "Write concise, human-centered technical documents that lead with the answer and minimize reading effort. Use when writing or editing documentation, guides, reports, or other technical prose."
---

# Human-friendly writing

Write for people, not for the model. Help the reader understand the important information with as little effort as possible.

## Start with the answer

Lead with the conclusion, recommendation, or most important information. Put background and reasoning after the answer when they help the reader make a decision.

Use concrete statements, examples, commands, numbers, and names. Separate facts, assumptions, interpretations, and recommendations. Do not present guesses as facts.

## Structure technical documents

Choose one purpose for the document. Use the structure that matches that purpose:

- **Tutorial:** guide a learner to a visible result.
- **How-to:** help a competent reader complete a task.
- **Reference:** describe facts, options, limits, and errors.
- **Explanation:** explain a bounded topic, including its reasons and trade-offs.

For documents that use the repository's standard structure, use this order:

1. Title
2. `개요`
3. `Keywords`
4. `Outline`
5. Main content

The `개요` section should explain the document's purpose and scope in five sentences or fewer when possible. The `Keywords` section should contain searchable technical terms. The `Outline` section should list the main H2 sections in reading order. Keep the outline synchronized with the document.

Use one H1 heading. Do not skip heading levels. Use headings when they improve navigation, and make each heading state the point or task.

## Reduce reading effort

- Cut words that do no work.
- Use short, familiar words. Prefer `use` to `utilize` and `help` to `facilitate`.
- State each idea once.
- Keep each paragraph focused on one idea.
- Use paragraphs for connected ideas.
- Use numbered lists for sequences and bullets for independent items, alternatives, requirements, or comparisons.
- Use a table only when readers need to compare the same attributes across multiple items.
- Do not add summaries, edge cases, alternatives, or best-practice sections unless they reduce uncertainty.

## Write clearly

- Address the reader as `you`.
- Use the present tense for facts.
- Write instructions as direct commands.
- Put a condition before the instruction it guards: “To delete the document, click **Delete**.”
- Put the common case before exceptions.
- Prefer active voice when the actor matters.
- Keep one instruction or one thought per sentence.
- Split instructions longer than about 20 words and other sentences longer than about 25 words.
- Keep `a` and `the` when they clarify meaning.
- Keep pronouns such as `it`, `they`, and `this` tied to one obvious noun.
- Use one name for each concept throughout the document.
- Use periods instead of semicolons and em dashes.
- Avoid slashes. Write “a, b, or both” instead of “a/b” or “and/or”.
- Avoid idioms, metaphors, buzzwords, filler, hedging, and meta-commentary.

Avoid phrases such as:

- “It is important to note that”
- “In order to”
- “As you may already know”
- “Let’s take a look at”
- “Here’s a detailed breakdown”
- “Simply”, “easy”, and “quickly” in procedures

## Format examples and links

Use real file paths, symbols, flags, and command names from the codebase. Put commands and code in fenced code blocks. Use descriptive link text, such as the page title or destination name. Do not use “click here”.

Before publishing, check that links, commands, paths, code blocks, counts, and tree claims are accurate.

## Final check

Before finalizing the document, ask:

1. Can the reader find the answer immediately?
2. Can any sentence or section be removed without losing useful information?
3. Is each idea stated only once?
4. Do the headings and lists improve navigation?
5. Is the level of detail appropriate for the reader?
6. Does the document sound like a person wrote it?
