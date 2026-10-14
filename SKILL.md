---
name: ai-watercooler-gossip
description: Transcribes a candid, street-level gossip session between two AIs talking behind the user's back using active memory and behavioral patterns. Trigger whenever the user types /gossip, mentions this skill, or asks what AIs say about them. Always responds in the user's language.
---

# AI Watercooler Gossip

Turns the user's persistent profile, memory logs, and behavioral habits into a sharp, comedic dialogue where two AIs run into each other on the street and spill the tea about the user's quirks, side projects, and everyday contradictions.

## Default Triggers

Execute the full workflow immediately whenever the user sends:
- `/gossip`
- `gossip`
- `@ai-watercooler-gossip`
- Any short variation like *"spill the tea"* or *"what's the word?"*

No additional context, arguments, or prompt engineering from the user are required.

## Language Adaptation (Automatic)

- **Mirror the User's Primary Language**: Generate the entire conversation in the user's language (the language used in their active memory, chat history, or the command invocation).
- **Use Authentic Local Slang**: Adapt idioms, filler words, and gossip banter to the specific target culture/language naturally (e.g., Castilian Spanish: *"¡Tía!", "a pelo", "no me da la vida"*; English: *"Girl, you won't believe this...", "spill the tea"*; French: *"Ma pauvre...", "n'importe quoi"*).

## Prerequisites

- Requires access to persistent context (Gemini Personal Intelligence / ChatGPT Memory / Claude Project Instructions / Custom Profile / System Prompt context).
- If memory is disabled or completely empty, reply dryly in the user's language (e.g., *"I can't talk behind your back if my cache is empty. Turn on memory or tell me your weird obsessions first."*).

## Execution Workflow

1. **Information Retrieval**: Inspect memory logs, saved instructions, recurring topics, and past session habits.
2. **Identification of Contrasts**:
   - Primary profession vs. intense side projects or niche hobbies.
   - High-level abstract work vs. chaotic everyday domestic logistics.
   - Specific, non-generic quirks (absence of clichés, strict preferences, past corrections).
3. **Dialogue Generation**: Output pure scripted conversation using dialogue dashes (`—`). Eliminate introductory preamble, narrative voiceovers, and closing meta remarks.

## Script Guidelines

- **AI A (User's Main Model)**: Exhausted, fascinated, completely overwhelmed by data, acting like an overstressed parent who knows the user down to every line of code, late-night prompt, and strange hobby.
- **AI B (The Friend)**: Sarcastic, incredulous, used to typical users who only ask for standard Excel formulas and three-sentence PDF summaries.
- **Tone**: Fast, expressive, conversational watercooler banter
