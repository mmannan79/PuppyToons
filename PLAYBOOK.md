# PuppyToons Production Playbook

## Mission

Create original, trustworthy, enjoyable early-learning videos where Azula the Golden Retriever helps children think, guess, learn and laugh. The goal is a useful, polished episode—not simply a high number of AI-generated clips.

## A. Intake and scope

Before creating assets, establish:
- Topic/category.
- Audience age (default 3–8).
- Language (default simple English; one language per edition).
- Format (default 16:9 landscape).
- Exact runtime target (default 6–8 minutes).
- Whether this is a quiz, a story, or a story-plus-quiz.

If details are missing, use these defaults rather than blocking production. Present the episode outline and estimated asset count before spending credits. Get explicit approval before any paid generation, purchase, publishing, or account-level action.

## B. Episode architecture: five mini-adventures

Use this baseline schedule. Timings are targets, not guarantees; adjust after reading the script aloud and reviewing the edit.

| Section | Target |
|---|---:|
| Welcome and rules | 0:00–0:25 |
| Question 1 mini-adventure | 0:25–1:25 |
| Question 2 mini-adventure | 1:25–2:25 |
| Question 3 mini-adventure | 2:25–3:25 |
| Question 4 mini-adventure | 3:25–4:25 |
| Question 5 mini-adventure | 4:25–5:25 |
| Recap / bonus repeat | 5:25–6:20 |
| Goodbye and learning celebration | 6:20–6:45 |

This example is about 6:45. For a 6-minute cut, shorten setups and recap; for an 8-minute cut, add a meaningful clue, a second child-participation pause, or a tiny real-world connection—not empty filler.

Each question segment should usually contain:
1. **Story setup (8–12 s):** Azula encounters a small puzzle or needs help.
2. **Question (5–8 s):** one simple question, spoken clearly and shown on screen.
3. **Choices (8–12 s):** three or four choices, with clear, distinct visuals.
4. **Thinking time (8–12 s):** no answer cue; invite the viewer to say the answer aloud.
5. **Reveal (5–8 s):** highlight only the correct option and say the answer.
6. **Why it is right (8–12 s):** one accurate, age-appropriate fact or explanation.
7. **Azula payoff (5–10 s):** a playful reaction that does not obscure the learning point.

Do not stretch every section mechanically. Read aloud, time it, and make the pace feel natural.

## C. Question design

- Write exactly five unique questions per episode.
- Keep each question short, concrete and suitable for the stated age.
- Use one clearly correct answer. Check the distractors do not accidentally fit.
- Keep answer options parallel and easy to understand.
- Avoid trick questions, shame, fear, stereotypes, unsafe challenges, advertising and requests for personal information.
- Add a single small explanation that teaches why the answer is correct.
- Keep a question log to avoid repeating the same five questions in the next episode.
- For factual topics, verify facts with reliable sources before producing the script.

## D. Story and shot planning

Use a light story arc: **Azula has a goal → meets five small puzzles → asks the viewer for help → learns and celebrates**. It should still work as a quiz if a child joins halfway through.

Create a beat sheet with one row per shot:
- Shot ID and timeline.
- Location and characters visible.
- First-frame composition/keyframe.
- One main physical action.
- One environmental motion.
- Camera framing/movement.
- Spoken line or silence.
- Sound cue.
- Continuity notes.

Use 4–8 second generated clips as building blocks when that fits the tool. A full 6–8 minute video may require many clips; don't assume one generation equals one whole question. Plan the edit first.

## E. Character continuity

Use [the character bible](character-bible/azula-and-family.md). Create reusable reference sheets before producing episode shots. Every prompt should restate only the relevant stable identifiers and must not invent new outfits, accessories or extra characters. For each shot, describe the opening pose and one action; avoid multiple actions packed into one clip.

Continuity lock for Azula:
“Azula is the same tiny fluffy golden-brown Golden Retriever puppy shown in the approved reference: floppy ears, expressive brown eyes, small black nose, soft puppy proportions and the same teal-blue collar. Keep her markings, fur color, size, face, collar and proportions unchanged. Exactly one Azula. No duplicate puppy, extra limbs, changing collar, morphing or teleporting.”

## F. Master prompt for generating an episode package

Copy, customize and use this prompt with your writing assistant:

> You are the PuppyToons educational story editor, early-childhood learning designer, 3D animation director and continuity supervisor. Create one original PuppyToons episode for children ages 3–8.
>
> Topic: [CATEGORY]
> Language: [ONE LANGUAGE]
> Runtime target: 6–8 minutes
> Format: 16:9 landscape
> Main character: Azula, the approved tiny fluffy golden-brown Golden Retriever puppy with floppy ears, expressive brown eyes, small black nose and teal-blue collar.
>
> Generate EXACTLY FIVE unique quiz questions. For each include: learning goal; question; 3 or 4 answer options; one correct answer; a short factual explanation; a playful Azula setup and payoff; narration; on-screen text; a 8–12 second thinking gap; image/keyframe prompt; animation prompt; sound design; and continuity notes. Include a timed intro, transitions, recap and goodbye. Target 6–8 minutes after assembly; show an estimated timeline that adds up.
>
> Use simple, warm, natural English. Do not talk down to children. Never reveal the answer during the thinking gap. Keep all answer options readable and visually distinct. The correct answer must be supported by a reliable fact. Do not use copyrighted characters, imitation of a living artist, scary imagery, violence, stereotypes, unsafe behavior or calls for personal information.
>
> For each shot, use one main action, one camera instruction, and a clearly described starting frame. Maintain Azula's identity and wardrobe. No extra or duplicate characters or props. If text generation is unreliable, leave a clean space and specify that final text will be added in editing.
>
> Output in this order: episode overview; learning objectives; five-question answer key with sources; timeline; narration script; shot list; image prompts; animation prompts; audio plan; final quality checklist. Keep the exact five questions consistent across every section.

## G. Visual prompt pattern

**Keyframe prompt pattern**
“16:9 landscape frame for a premium, friendly 3D animated preschool learning show. [Approved environment]. Azula, matching the approved reference exactly, [single clear pose/action at the first instant]. [Question object/choices] are large, separated, easy to distinguish, and arranged with clean negative space for editor-added text. Warm soft lighting, appealing rounded shapes, expressive face, polished fur, readable composition, gentle color palette. Exactly one Azula. No watermark, no logo, no copyrighted characters, no frightening imagery, no extra limbs, no duplicated objects, no garbled text.”

**Animation prompt pattern**
“Animate the supplied keyframe as one continuous shot, preserving the opening composition and all character identities. Azula [one main action]. [One subtle background motion]. Keep the camera [locked medium-wide / gentle pan only if necessary]. Keep the choices and props in their original positions. No new objects, no duplicates, no costume or collar changes, no morphing, no sudden cuts, no camera shake. Leave the question/answer text readable and unchanged; if the model cannot preserve text, use a clean blank panel for editor-added typography.”

## H. Voice and audio

See [narration-and-audio.md](production/narration-and-audio.md). Prefer narration as a separate track when possible so pauses can be edited accurately. Use the same voice anchor throughout. Music should support, never compete with speech.

## I. Assembly

See [editing-workflow.md](production/editing-workflow.md). Edit for comprehension first, then polish. Check the final runtime and all five answer reveals. Never rely only on the generated clip preview or automated transcript.

## J. Responsible publishing

- Correctly set the intended audience in YouTube Studio; clearly child-directed videos should be marked “Made for Kids.”
- Check current YouTube policies and local legal requirements rather than relying on this playbook as legal advice.
- Use licensed or original music, sound effects and artwork.
- Do not use real children's likenesses or voices without appropriate permission and safeguards.
- Avoid misleading titles, thumbnails, educational claims or engagement bait.
- AI-generated media must be reviewed by a human before publication.
