# PuppyToons AI Storytelling Playbook (v3)

A repeatable system for emotional, story-driven PuppyToons videos — 3D animated
short stories starring Azula and the Baker Family, built for YouTube Shorts,
TikTok, and Reels. This playbook adapts the viral AI-storytelling workflow
(character-locked 3D narration stories: hook → tension → twist → payoff) to
PuppyToons' audience: children ages 3–8 and their families. Every story is
wholesome, gentle, and kind — no villains, no fear, no meanness.

**Sources and adaptation notes.** This is an original PuppyToons workflow
informed by two sources, neither reproduced here:
- [From Idea to Viral Video: AI Storytelling — The Radio TV](https://theradiotv.net/from-idea-to-viral-video-ai-storytelling/) — the character-locked storytelling pipeline (story idea generator, script writer, character/scene visualization prompts, image-to-video motion prompts) and the hook-first retention structure. Its master prompts are summarized and re-authored below in original form for a kids audience.
- [PuppyToons repository — github.com/mmannan79/PuppyToons](https://github.com/mmannan79/PuppyToons) — the v1 production playbook (character continuity, Azula lock, beat-sheet planning) and the v2 quiz-card playbook. This v3 adds the *story* format alongside them.

Tool features, availability, pricing, and model names change; verify them in the
apps before production.

## 1. Channel identity (decide once, never change)

- **Main character:** Azula — tiny fluffy golden-brown Golden Retriever puppy,
  floppy ears, expressive brown eyes, small black nose, teal-blue collar.
  Azula appears in every story and looks identical every time.
- **Supporting cast (from the Baker Family sheet):** Mom Sarah, Dad David,
  Sister Maya (4, purple cape, yellow boots), Baby Brother Leo (9 months).
  They rotate by story; their looks never change.
- **Voice:** one warm adult female narrator, clear and gentle-paced, same
  voice in every video. (Current voice: Aria — feminine, American, warm.)
- **Format:** 9:16 vertical, 45–90 seconds, narrated throughout.
- **Rule:** never redesign Azula between videos. Small visual drift breaks the
  bond viewers build with her.

**Azula continuity lock (paste into every Azula prompt):**
"Azula: one tiny fluffy golden-brown Golden Retriever puppy, floppy ears,
expressive brown eyes, small black nose, rounded puppy proportions, teal-blue
collar. Preserve her face, fur, markings, scale and collar. Exactly one Azula;
no duplication, morphing, extra limbs or wardrobe changes."

## 2. The story engine (kid-safe viral structure)

Every story follows five beats. The article's viral territories (crime,
revenge, betrayal) are replaced with kid-safe equivalents:

**Kid-safe story territories** (rotate; never repeat twice in a row):
kindness to animals, courage when scared, honesty, helping family, friendship,
trying again after failing, sharing, saying sorry, welcoming someone new.

**The five beats:**
1. **Hook (0–3 sec):** one surprising or curious opening line + image that
   stops the scroll. Ask a question or state a small mystery.
   ("Azula found something in the garden… and it was MOVING.")
2. **Tension (3–25 sec):** a clear problem sized for a child — something lost,
   someone sad, a storm coming, a friend in trouble. Raise the stakes gently.
3. **Escalation (25–45 sec):** Azula tries to help; it gets a little harder.
   One complication only. Keep it warm, never frightening.
4. **Twist (45–60 sec):** a gentle surprise that reframes everything — the
   "scary" sound was a friend; the lost thing was closer than thought.
5. **Payoff (60–75 sec):** the problem solves with kindness. End on one clear,
   sayable moral. ("Being brave means helping, even when you feel scared.")

**Retention rules for kids:** one idea per scene; short sentences; name
feelings out loud ("Azula felt a little scared, but…"); repeat the story's
one lesson twice (middle and end); no scene longer than 10 seconds.

## 3. Master prompts (original — write with these, then generate)

### Prompt 1 — Story idea generator (seven ideas)

> You are a children's story editor for ages 3–8. Generate 7 ORIGINAL short
> video story ideas starring Azula, a tiny golden retriever puppy, and the
> Baker Family (Mom Sarah, Dad David, Maya age 4, baby Leo).
>
> Each idea follows: HOOK (one curious opening line, under 3 seconds spoken),
> TENSION (a gentle, child-sized problem), TWIST (a kind surprise that reframes
> the problem), PAYOFF (solved through kindness; one sayable moral).
>
> Rules: wholesome only — no villains, no fear, no meanness, no danger that
> isn't resolved. Rotate territories (kindness, courage, honesty, helping,
> friendship, persistence, sharing). Output: title, then Hook / Tension /
> Twist / Payoff, one block per idea. Then STOP and ask me to pick one.

### Prompt 2 — Script + beat writer (for the chosen idea)

> Write the complete voiceover script for the chosen Azula story. 130–200
> spoken words, 45–75 seconds. Natural warm narration, simple vocabulary,
> short sentences, strong verbs, zero filler.
>
> Structure: HOOK first (under 3 seconds) → TENSION → ESCALATION → TWIST →
> PAYOFF with the moral stated plainly at the end. Every beat must open a
> small curiosity loop ("But then…", "That's when…", "What happened next…").
>
> Then break the script into numbered BEATS (one beat per 8–10 seconds, 5–8
> beats total). For each beat: the exact narration lines, who is on screen,
> the one emotion of the beat, and one visual note. Beat numbering must stay
> fixed — Beat 1 = Scene 1 everywhere downstream.

### Prompt 3 — Scene visualization (one prompt per beat)

For each beat, write one image/video prompt containing:
1. Exact character names on screen + the Azula continuity lock (and Baker
   locks for family members present).
2. One clear action and one exact facial expression per character.
3. Environment, time of day, and lighting tied to the emotion
   (warm golden = safe/happy; soft blue-grey = worry; bright sun = payoff).
4. Camera: pick the shot that serves the beat — close-up for feelings, wide
   for discovery, low angle for the hero moment.
5. Fixed quality suffix on every prompt: "9:16 vertical, premium 3D family-film
   animation, soft realistic fur, expressive faces, gentle cinematic lighting,
   warm bright colors, simple uncluttered background, no text, no logos."

Negative (every prompt): morphing faces, extra limbs, duplicate characters,
costume changes, scary imagery, text or words in the image.

### Prompt 4 — Motion (one per scene, for the video tool)

> Animate as one continuous shot, 10 seconds, 9:16. Camera: [one move —
> slow push-in for emotion, gentle pan for discovery, locked for calm beats].
> Character motion: [one main action, continuous and smooth]. Face: [expression
> change across the clip, e.g., curious → eyes widen → soft smile]. Pacing:
> [gentle / building / joyful] to match the beat. Ambience note for the edit:
> [e.g., "soft wind + distant birds"; "rain patter"]. No new characters, no
> morphing, no text appearing. End on a stable frame.

Keep motion, camera, face, and pacing in every motion prompt. Sound (ambience,
SFX, music) is added in the edit, not generated in the clip.

## 4. Production pipeline (VideoExpress.ai)

1. **Write first.** Run Prompts 1–2, pick the story, lock the beats. Never
   generate before the script exists.
2. **Generate in batches of 5.** Text To Video, 9:16 vertical, 10 seconds per
   clip, Advanced Mode on, prompt enhancement OFF, public gallery OFF. One
   clip per beat (Prompt 3 + Prompt 4 combined). 5–8 clips cover a full story.
3. **Voiceover separately.** Generate the full narration as its own audio in
   the locked voice (same voice every video). Separate audio lets the edit
   place pauses exactly.
4. **Edit in story order:** lay narration first, cut clips to the beats, trim
   any dead air, simple cuts (no flashy transitions), slow subtle zoom where a
   shot feels static, warm color grade.
5. **Sound:** one gentle music bed (ukulele/soft piano/marimba) kept well
   under the narration; add 2–3 soft SFX at key beats (gasp, chime, birdsong).
   Mix order: narration on top, SFX under it, music lowest.
6. **Thumbnail/poster:** the twist or payoff frame, Azula's most expressive
   face, 3–5 word caption.

## 5. QC gates

- **Gate 1 — Story:** moral is kind and sayable; no fear/meanness unresolved;
  twist is gentle; hook lands in 3 seconds.
- **Gate 2 — Continuity:** Azula identical in every scene (lock pasted);
  family members match the sheet; no duplicates or costume changes.
- **Gate 3 — Craft:** no text baked into images; no morphing/jitter; narration
  and clips in sync; music never covers the voice; 45–90 sec total.

## 6. Publishing (YouTube Shorts / TikTok / Reels)

- Title: story title + one emoji; first line of description restates the hook.
- Hashtags: 3–5 (#puppytoons #azula #kidstories …).
- Mark as child-directed per current platform rules; disclose AI-generated
  content where the platform requires it.
- Post cadence: the system is built for volume — one finished story beats
  three half-made ones.

---

## Worked example — Story 001: "Azula and the Lost Baby Bird"

*Original story written for this playbook. Beats 1:1 with scenes.*

**Script (narration):**
"Azula found something in the garden… and it was MOVING. [Beat 1]
Under a big green leaf, a tiny baby bird was shivering. All alone. The sky
was turning grey. [Beat 2]
'Don't worry, little one,' Maya whispered. She and Azula built a tiny shelter
of leaves and twigs. But then… the wind began to howl. [Beat 3]
Something big was rustling in the bushes! Azula's ears stood straight up…
It wasn't a monster. It was the mama bird — looking everywhere for her baby!
[Beat 4]
Azula gently nudged the little bird toward its mama. The sun peeked out. And
the two birds chirped the happiest song in the whole garden. [Beat 5]
That evening, Maya gave Azula the biggest belly rub. Because being brave
doesn't mean not feeling scared — it means helping anyway. [Beat 6]"

**Scenes (9:16, 10 sec each — Prompts 3+4 combined):**

- **Scene 1 (Hook):** Extreme close-up, Azula in sunny garden, ears perked,
  eyes widening toward camera; leaves rustle at frame edge. Warm golden light.
  Motion: slow push-in; Azula's head tilts, nose twitches. + Azula lock.
- **Scene 2 (Tension):** Low wide shot under a big leaf: tiny baby bird
  shivering; Azula noses the leaf aside gently, soft worried eyes. Sky greying.
  Motion: gentle pan; bird trembles, Azula blinks kindly. + Azula lock.
- **Scene 3 (Escalation):** Medium shot: Maya (purple cape, yellow boots)
  kneeling, placing twigs; Azula carries a leaf in her mouth; wind lifts
  leaves. Motion: handheld sway; Maya smiles determined, Azula wags once.
  + Azula lock + Maya lock.
- **Scene 4 (Twist):** Bushes fill frame, dark shape moves — cut to reveal:
  worried mama bird hopping out, wings half open, calling. Azula sits back,
  surprised then relieved. Motion: quick pan to reveal, then settle; Azula's
  ears drop then lift. + Azula lock.
- **Scene 5 (Reunion):** Wide warm shot: Azula nudges baby bird with her nose
  toward mama bird; sun breaks through clouds; birds touch beaks, chirping.
  Motion: slow push-in; Azula's tail wags happily. Golden light returns.
  + Azula lock.
- **Scene 6 (Payoff):** Garden picnic at sunset: Maya gives Azula a belly rub,
  Azula blissful on her back; Sarah, David, Leo smiling nearby; birds on a
  branch above. Motion: locked calm frame, leaves sway softly. + full family
  locks.

**Sound:** narration (locked voice) + gentle acoustic music bed + SFX:
leaf-rustle (Sc.1), soft wind (Sc.3), happy chirps (Sc.5), warm chime (Sc.6).
