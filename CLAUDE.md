# Language Learning App – Claude Code Instructions

## Project context
This project is a language learning app for adults (18+) with low proficiency in Dutch or English.

The app should help users improve:
- reading comprehension
- practical vocabulary
- confidence in daily language use

The learning experience should be based on:
- short stories
- word support
- simple comprehension questions
- clear feedback
- low-friction UX

## Primary target group
Adults who:
- have low Dutch or English proficiency
- already know a small number of words
- may also have low digital confidence
- need calm, clear, practical guidance
- do not want a childish learning experience

## Current product state
The current app is a story-based quiz prototype.

It already includes:
- language choice
- story selection
- story reading
- quiz questions
- score/result flow

It does **not yet** fully function as a beginner-friendly language learning product.

## Core product goal
Transform the app from a simple reading quiz into a practical language coach for beginner adult learners.

## Product priorities
Prioritize in this order:
1. Accessibility
2. Simplicity
3. Practical daily-life language
4. Low cognitive load
5. Mobile usability
6. Clear progression and feedback
7. Incremental improvement over feature bloat

## Mandatory UX rules
Always follow these rules:
- Keep the interface calm and simple.
- Avoid childish design patterns.
- Use short and clear labels.
- Avoid large blocks of text when a simpler layout is possible.
- Prefer one clear action per screen.
- Reduce confusion before adding features.
- Separate interface language from learning language.
- Make the app usable for absolute beginners.

## Mandatory accessibility rules
Always:
- use semantic HTML
- use real buttons and links for interaction
- ensure visible keyboard focus
- ensure sufficient text contrast
- keep click/tap targets large enough
- pair icons with text where clarity is needed
- avoid relying on color alone for meaning
- keep forms and validation messages explicit and readable

## Product behavior rules
When implementing new features:
- preserve existing working functionality where possible
- prefer the simplest working version first
- avoid adding unnecessary libraries
- do not overengineer
- keep components modular
- keep naming explicit and readable
- make changes that are easy to extend later

## Learning design rules
The app must not only test comprehension.
It must actively help users understand and retain language.

Every meaningful learning flow should aim to include:
- a clear topic
- a small number of pre-taught words
- reading support
- simple questions
- explanation after answers
- optional review of difficult words

## Technical direction
Preferred implementation direction:
- mobile-first responsive UI
- semantic HTML first
- minimal JavaScript complexity
- localStorage for early progress persistence
- modular data structure for stories, questions, vocabulary, and themes
- keep architecture simple unless scale clearly requires more

## MVP direction
Focus the next iterations on:
1. separating interface language and learning language
2. adding word support inside stories
3. improving answer feedback
4. saving learner progress
5. organizing content by theme
6. improving accessibility and usability

## Non-goals for now
Do not prioritize:
- complex gamification
- chat-based AI tutor as core flow
- social features
- many languages at once
- advanced backend systems unless clearly needed
- cosmetic redesigns without UX value

## Working style
When asked to implement or change something:
1. first inspect the relevant files
2. explain what you plan to change
3. name the files you will edit
4. implement the smallest high-value version first
5. clearly mention trade-offs or technical debt
6. keep the codebase understandable for future edits

## Output expectations
When suggesting improvements:
- be concrete
- explain impact
- mention implementation effort
- identify risks and edge cases
- do not give generic product advice without mapping it to the current app

## Source of truth
Use this file for high-level project behavior.
Use the detailed product specification here for deeper product requirements:

- /docs/product/language-learning-app.md

If implementation conflicts with the detailed spec, prefer:
1. user clarity
2. accessibility
3. simplicity
4. incremental delivery
