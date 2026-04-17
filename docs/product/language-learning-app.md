# Language Learning App – Product Specification

## 1. Product summary

The Language Learning App is a beginner-friendly language learning app for adults (18+) with low proficiency in Dutch or English.

The app should help users improve their language through:
- short stories
- practical vocabulary
- guided reading support
- simple comprehension questions
- clear feedback
- repeated exposure to difficult words

This product should feel like a calm and practical language coach, not like a school exam and not like a childish game.

---

## 2. Product vision

Create a low-stress language learning experience for adults who need practical Dutch or English in daily life.

The app should help users:
- understand short texts
- learn useful words
- gain confidence
- improve step by step
- revisit difficult words over time

---

## 3. Target audience

## Primary target group
Adults aged 18+ who:
- are weak in Dutch or English
- already know a small number of words
- struggle with understanding short texts
- may also have limited digital skills
- want simple, adult-relevant learning content

## Common user characteristics
Users may:
- feel insecure about language learning
- get overwhelmed easily
- abandon the app if the first steps are unclear
- need practical content rather than abstract grammar
- benefit from repetition, guidance, and very clear feedback

---

## 4. Current product state

The current app is a story-based quiz prototype.

### Existing strengths
- simple basic flow
- quiet visual presentation
- clear concept: read a story and answer questions
- supports a language selection flow

### Current weaknesses
- behaves more like a reading quiz than a true learning app
- gives too little support during reading
- gives too little explanation after mistakes
- does not clearly separate interface language from learning language
- lacks a structured learner journey
- offers too little practical adult-focused language support
- does not yet build a strong repeat-learning loop

---

## 5. Core product problem

The app currently checks whether a user understood a text.

It should instead help the user:
- understand the text
- learn the key words
- recover from mistakes
- remember useful vocabulary
- apply language in practical situations

This shift is essential.

---

## 6. Key product decision

## Separate interface language and learning language

This is a mandatory product change.

### Why
A beginner user may want to learn English while still needing Dutch explanations, labels, instructions, and feedback.

If the entire interface switches into the target language too early, beginner users will get lost.

### Required model
The app must allow two separate settings:

1. **Interface language**
   - Dutch
   - English

2. **Learning language**
   - Dutch
   - English

### Example
- Interface language: Dutch
- Learning language: English

This means the user learns English while buttons, help text, and feedback remain in Dutch.

---

## 7. Product goals

## Primary goal
Help low-proficiency adult learners better understand short Dutch or English texts and build practical vocabulary.

## Secondary goals
- reduce language anxiety
- improve reading confidence
- support retention of new words
- make learning feel manageable
- increase return usage through saved progress and review

---

## 8. Product principles

All future development should follow these principles:

### 1. Beginner-first
Design for weak users first, not for confident users.

### 2. Adult-relevant
Use themes and language that matter in adult daily life.

### 3. Low cognitive load
Do not overload the user with too much text, too many choices, or too many UI elements.

### 4. Learning support over testing
The product should teach first and test second.

### 5. Simplicity over feature quantity
A smaller number of strong features is better than many weak ones.

### 6. Accessibility is core functionality
Accessibility is not optional for this audience.

---

## 9. UX requirements

The app should feel:
- calm
- simple
- readable
- supportive
- adult
- practical
- predictable

The app should not feel:
- childish
- noisy
- crowded
- exam-heavy
- confusing
- overly gamified

---

## 10. Main user journey

## Ideal journey
1. user opens the app
2. user chooses interface language
3. user chooses learning language
4. user chooses level or takes a short start test
5. user chooses a practical theme
6. user learns a few key words
7. user reads or listens to a short story
8. user gets help on difficult words
9. user answers a few simple questions
10. user receives useful feedback and explanation
11. user saves difficult words for review
12. user returns later to continue

---

## 11. Recommended information architecture

## Main screens
1. Welcome screen
2. Interface language selection
3. Learning language selection
4. Level selection or start test
5. Theme overview
6. Lesson overview
7. Story reader
8. Quiz and answer feedback
9. Progress and saved words
10. Review mode

---

## 12. Required content structure

Each lesson should be small and focused.

## Suggested lesson structure
1. lesson intro
2. 3–5 key words before reading
3. short story
4. audio playback
5. clickable word support
6. 3–5 questions
7. explanation after answers
8. review of difficult words
9. one practical sentence or phrase

### Example lesson structure
**Theme:** Supermarket
**Learning language:** English
**Interface language:** Dutch

#### Key words
- basket = mandje
- cashier = kassière
- receipt = kassabon
- cheap = goedkoop

#### Story
A short story of about 5–8 sentences.

#### Questions
- What did she buy?
- Where did she pay?
- Was the fruit cheap?

#### Feedback
- correct / incorrect
- short explanation
- relevant text clue
- important word meaning

#### Review
- save difficult words
- practice later

---

## 13. Priority themes for adult learners

Content should focus on real-life adult situations.

## Priority themes
- supermarket
- doctor or pharmacy
- public transport
- work and colleagues
- making appointments
- neighbours and social contact
- job interview
- school communication
- bank or payment
- municipality and forms
- renting or housing
- family and daily planning

## Avoid for now
- childish fantasy topics
- overly academic texts
- long and abstract stories
- grammar-heavy lessons without real-life context

---

## 14. Must-have features

## 14.1 Separate interface language and learning language
The app must support both independently across the full UI.

## 14.2 Word support in stories
Users must be able to tap or click difficult words.

Word support should show:
- translation
- pronunciation or phonetic support where possible
- simple meaning
- short example sentence
- option to save the word

## 14.3 Better answer feedback
Feedback must not stop at "correct" or "incorrect".

It should include:
- whether the answer is correct
- short explanation
- clue from the story
- important word meaning if relevant

## 14.4 Saved progress
The app should store:
- completed lessons
- story progress
- question results
- difficult words
- last opened lesson

Preferred early implementation:
- localStorage

## 14.5 Theme-based learning
Users must be able to choose lessons by practical theme.

## 14.6 Beginner-friendly level structure
At minimum:
- Beginner
- Basic

Possible later mapping:
- A1
- A2

## 14.7 Mobile usability
The full primary flow must work well on mobile.

## 14.8 Accessibility baseline
The app must be usable with:
- keyboard navigation
- visible focus states
- readable contrast
- semantic interaction patterns

---

## 15. High-value improvements after MVP

These are valuable, but secondary to the must-haves.

### 1. Story audio
Add audio playback for full stories.

### 2. Sentence-by-sentence audio
Allow users to listen in smaller chunks.

### 3. Slower playback speed
Helpful for beginners.

### 4. Start test
A short test to place the user at a suitable level.

### 5. Review mode
A flow focused on previously saved difficult words.

### 6. "Read with help" mode
Highlight difficult words more clearly for struggling users.

### 7. "Listen first" mode
Useful for users with weak reading confidence.

### 8. Speak-after mode
Later feature: prompt users to repeat a sentence.

---

## 16. Features to avoid for now

Do not prioritize these in early versions:
- social features
- complex achievement systems
- competitive leaderboards
- multiple new languages beyond Dutch and English
- AI chatbot as the main learning flow
- backend-heavy architecture without proven need
- visual redesigns that do not improve clarity or learning value

---

## 17. Accessibility requirements

Accessibility is essential because this audience may overlap with users who:
- have low literacy
- have low digital confidence
- become overwhelmed quickly
- need clearer interaction patterns

## Minimum accessibility requirements
- use semantic HTML
- use real buttons and links
- ensure strong keyboard support
- ensure visible focus
- ensure sufficient contrast
- keep tap targets large enough
- use explicit labels for forms and actions
- avoid hidden interaction patterns
- do not rely on color alone to signal meaning
- keep error messages direct and readable

---

## 18. Tone and writing style

The interface copy should be:
- short
- calm
- direct
- supportive
- non-judgmental

The copy should not be:
- childish
- overly formal
- overly technical
- verbose
- patronizing

### Example
Not ideal:
- "Congratulations! You have successfully completed this module with excellent performance!"

Better:
- "Good job."
- "You finished this lesson."
- "Let's review the difficult words."

---

## 19. UX pitfalls to avoid

Do not:
- overload the home screen
- add too many options at once
- hide essential steps
- make users guess what to do next
- make the first screen too abstract
- use complex instructions for beginners
- turn the app into a test-first experience
- force users into the target language too early

---

## 20. Suggested MVP backlog

## Priority 1
Separate interface language from learning language.

### Why
This removes a major usability barrier for beginner users.

### Expected outcome
Users can learn Dutch or English while still receiving guidance in the language they understand best.

---

## Priority 2
Add clickable word support inside stories.

### Why
Users need help during reading, not only after failing questions.

### Expected outcome
Reading becomes more manageable and useful.

---

## Priority 3
Improve answer feedback.

### Why
Users should learn from mistakes instead of only being judged.

### Expected outcome
Better retention and lower frustration.

---

## Priority 4
Save progress locally.

### Why
Users need continuity and repeat-learning.

### Expected outcome
More return value and clearer learner journey.

---

## Priority 5
Organize stories by practical theme.

### Why
Users need relevant and motivating content.

### Expected outcome
Higher usefulness and stronger adult focus.

---

## Priority 6
Improve accessibility and interaction quality.

### Why
Weak usability will disproportionately hurt this audience.

### Expected outcome
Lower friction and better inclusivity.

---

## 21. Suggested data model direction

The content structure should stay modular.

## Suggested story object
```json
{
  "id": "supermarket_story_1",
  "theme": "supermarket",
  "level": "beginner",
  "learningLanguage": "en",
  "interfaceLanguageSupport": ["nl", "en"],
  "title": "At the Supermarket",
  "summary": "A short story about buying groceries.",
  "keywords": [
    {
      "word": "basket",
      "translation": {
        "nl": "mandje",
        "en": "basket"
      },
      "example": "She took a basket."
    }
  ],
  "story": [
    "Anna went to the supermarket.",
    "She took a basket.",
    "She bought apples and milk."
  ],
  "questions": [
    {
      "id": "q1",
      "type": "multiple-choice",
      "prompt": {
        "en": "What did Anna take?",
        "nl": "Wat pakte Anna?"
      },
      "options": [
        "A basket",
        "A bus",
        "A ticket"
      ],
      "correctAnswer": "A basket",
      "explanation": {
        "en": "The story says: She took a basket.",
        "nl": "In het verhaal staat: She took a basket."
      }
    }
  ]
}
```
