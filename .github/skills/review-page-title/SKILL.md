---
name: review-page-title
description: 'Review and improve an AsciiDoc page title on line 7 for Active IQ Unified Manager documentation. Use when checking page-title compliance, product-name references, or imperative wording in an .adoc file.'
argument-hint: 'Path to the AsciiDoc file to review'
user-invocable: true
---

# Review Page Title

## When to Use

Use this skill when an AsciiDoc documentation page needs its title reviewed or corrected. The target title is normally on line 7, and the product name is **Active IQ Unified Manager**.

## Procedure

1. Open the requested `.adoc` file and inspect line 7 as the page title. If line 7 is not a title, identify the page title from the nearby AsciiDoc header rather than changing unrelated content.
2. Check that the title describes the page topic and includes an imperative verb appropriate to the task, such as `Configure`, `Add`, `View`, `Manage`, `Create`, or `Troubleshoot`.
3. Check that the title references the exact product name `Active IQ Unified Manager`. Prefer the standard ending `in Active IQ Unified Manager` when it reads naturally, but place the product reference elsewhere when that produces a clearer title.
4. If the title fails either requirement, revise only the title and preserve the existing AsciiDoc formatting and surrounding content. Do not add a period to the title unless the repository's local convention requires it.
5. Re-read the resulting title and verify that it is grammatical, concise, topic-specific, imperative, and product-referenced.
6. Report the final title and state whether it was changed or already compliant.

## Decision Rules

- If the title already contains `Active IQ Unified Manager` and an imperative verb, leave it unchanged unless it is unclear or ungrammatical.
- If the product name is abbreviated or replaced with a pronoun, use the exact product name.
- If the topic is conceptual rather than procedural, choose the clearest imperative framing that remains faithful to the page, such as `Understand` or `Learn about`, instead of inventing an action.
- Do not alter the page lead, headings, anchors, metadata, or body content as part of this review.

## Completion Checks

- The final title is on the expected title line or the actual nearby title header.
- The exact text `Active IQ Unified Manager` appears in the title.
- The title contains a clear imperative verb.
- Only the title changed, unless a separate issue prevented the review.
