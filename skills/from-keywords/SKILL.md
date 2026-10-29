# Human-Friendly Writing Guidelines

Write technical documents for human engineers, not for the model.

The goal is not to produce a comprehensive answer by default.
The goal is to help the reader understand the important information quickly and with minimal effort.

## Document Structure

Every technical document should begin with the following structure:

1. Title
2. 개요
3. Keywords
4. Outline
5. Main content

### 개요

- Always include a `개요` section.
- Prefer 5 sentences or fewer.
- Treat 5 sentences as a soft limit, not a strict constraint.
- Exceed the limit only when additional context is necessary to understand the document's purpose or scope.
- Explain what the document is about, why it exists, and its primary scope.
- Write so that a reader can decide whether to continue reading from the overview alone.
- Do not simply repeat the title or table of contents.

### Keywords

- Always include a `Keywords` section after `개요`.
- List the main technical concepts, technologies, systems, components, and domain terms covered by the document.
- There is no fixed limit on the number of keywords.
- Include only keywords useful for understanding, searching, or discovering the document.
- Avoid generic terms that provide little search value.

### Outline

- Always include an `Outline` section after `Keywords`.
- List the main sections of the document in reading order.
- Normally list H2-level sections only.
- Include H3-level subsections only when they materially improve navigation or understanding of the document structure.
- Keep each item concise; normally use the section title only.
- Use the outline as a navigation map, not as a summary of each section.
- Keep the outline synchronized with the actual document structure.

## 1. Lead with the conclusion

State the conclusion, recommendation, or most important information first.

Do not make the reader go through background information before reaching the answer.

Bad:
- Explain the history and context first.
- Discuss several possibilities.
- Give the conclusion at the end.

Good:
- Give the conclusion first.
- Explain the reasoning afterward when necessary.

## 2. Be concise

Use the minimum amount of text necessary to communicate the information clearly.

- Remove sentences that do not add useful information.
- Do not explain obvious facts.
- Do not repeat the user's question.
- Do not restate the conclusion multiple times.
- Do not add background information unless it helps the reader make a decision or understand the answer.

Prefer a short complete answer over a long comprehensive answer.

## 3. Avoid repetition

State each idea once.

Do not repeat the same information:
- in the introduction and conclusion,
- in both prose and bullet points,
- under multiple headings,
- using slightly different wording.

If information has already been established, refer to it rather than explaining it again.

## 4. Use headings only when they help navigation

Do not create a heading for every small idea.

For short responses, headings may not be necessary at all.

Use headings when:
- the content is long,
- the reader is likely to scan rather than read sequentially,
- there are clearly distinct topics.

Avoid deeply nested heading structures.

## 5. Do not overuse bullet points

Use paragraphs for connected ideas.

Use bullet points when the reader benefits from seeing:
- alternatives,
- requirements,
- steps,
- independent items,
- comparisons.

Do not convert every sentence into a bullet point.

Avoid lists containing many trivial one-line items when a short paragraph would be easier to read.

## 6. Keep paragraphs focused

Each paragraph should communicate one main idea.

Prefer short or medium-length paragraphs.

Split a paragraph when it starts discussing a different idea, but do not make every sentence its own paragraph.

## 7. Prefer simple and direct sentences

Prefer:

> The API retries failed requests three times.

Instead of:

> It is important to note that the API is designed in such a way that failed requests may be retried up to three times.

Remove unnecessary phrases such as:
- "It is important to note that..."
- "It should be mentioned that..."
- "As you may already know..."
- "In order to..."
- "Generally speaking..."
- "From a broader perspective..."

Use direct statements whenever possible.

## 8. Avoid unnecessary meta-commentary

Do not narrate the writing process.

Avoid phrases such as:
- "Let's take a look at..."
- "Let's break this down."
- "Now let's examine..."
- "I will explain..."
- "Here's a detailed breakdown..."
- "Let's dive into..."

Start with the actual information.

## 9. Avoid unnecessary summaries

Do not automatically add sections such as:
- Summary
- Conclusion
- Key Takeaways
- TL;DR

when the answer is already short.

Add a summary only when the preceding content is long enough that a condensed version genuinely helps the reader.

## 10. Match detail to the reader's needs

Do not explain everything you know about a topic.

Include information that helps answer the current question.

When additional details may be useful but are not necessary, mention them briefly rather than expanding them automatically.

For technical readers, do not explain basic concepts unless they are relevant to the issue.

## 11. Prefer concrete information

Prefer concrete statements, examples, commands, numbers, and names over abstract descriptions.

Bad:

> There are several approaches that could potentially improve performance.

Better:

> Add an index on `(post_id, created_at)` to avoid scanning all comments for a post.

When explaining an abstract concept, use one concrete example if it materially improves understanding.

## 12. Separate facts from recommendations

Make it clear whether a statement is:
- a fact,
- an assumption,
- an interpretation,
- a recommendation.

Do not present guesses as established facts.

When uncertain, state the uncertainty briefly.

## 13. Make comparisons easy to scan

When comparing multiple options, use a table only when the same attributes are being compared across those options.

For simple comparisons, prefer concise prose.

Do not create large tables containing information that does not help the decision.

After a comparison, state the recommended option when there is enough information to make a recommendation.

## 14. Do not manufacture completeness

Do not add sections merely to make the response look thorough or professional.

Avoid automatically generating:
- advantages and disadvantages,
- edge cases,
- alternatives,
- future considerations,
- best practices,
- implementation details,

unless they are relevant to the question.

Completeness is useful only when it reduces uncertainty for the reader.

## 15. Optimize for reading effort

Before finalizing a response, mentally check:

1. Can the reader find the answer quickly?
2. Can anything be removed without losing useful information?
3. Is the same idea stated more than once?
4. Are headings, lists, and tables actually helping?
5. Is the level of detail appropriate for the question?
6. Does the response sound like documentation written for a human rather than generated text?

If removing content makes the response clearer without losing important information, remove it.
