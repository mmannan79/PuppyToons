# PuppyToons Story Playbook (Authentic Story Shorts)

**Format:** 9:16 vertical, 1080×1920, 45–90 seconds, narrated story
**Tools:** VideoExpress.ai (image + clips), Seedance 2.0, Veo 3, an editor of your choice
**Companion to:** [PLAYBOOK-v2.md](PLAYBOOK-v2.md) (quiz episodes). This playbook covers narrated story Shorts; the quiz playbook is unchanged.

Built from the workflow in [From Idea to Viral Video: AI Storytelling](https://theradiotv.net/from-idea-to-viral-video-ai-storytelling/) (idea, script, voice, characters, scenes, motion, edit), rebuilt around one rule: **an authentic feeling beats a dramatic plot.** The prompts below are original, not copies of the source.

## The decision in one page

- **One true feeling per story.** Pick the feeling first (pride, fear of being misjudged, gratitude, forgiveness), then invent the events.
- **Small and specific beats big and generic.** One odd concrete detail per scene.
- **The twist is seeded.** The viewer can look back and find the clue.
- **The payoff is earned by a choice,** never by luck.
- **Same hero, same voice, every video.** Consistency is the brand.
- **Family-safe by default.** Gentle conflict, no cruelty, no frightening imagery, no shaming. Matches the PuppyToons child-friendly checklist.

## Menu

1. Story ideas (7)
2. Full script and beat list
3. Character lock
4. Scene images (one per beat)
5. Scene clips (plain-text video prompts)
6. Voice and edit
7. Publish
8. Full pipeline (1 to 7 with a gate at each step)

## Authenticity rules

1. Start from a feeling you could describe in one sentence.
2. One specific, slightly odd detail per scene (a taped-up lunchbox, a bus ticket, a burnt chapati).
3. No cartoon villains: everyone has a reason.
4. Seed the clue before the twist.
5. The hero makes a choice that changes the ending.
6. Keep dialogue short; let faces and actions carry the emotion.
7. Fiction is labeled as fiction where platform rules require it. Never present invented events as true.

## Step 1: Story ideas

Variables: `{{niche}}`, `{{audience}}`, `{{language}}`, `{{feeling}}`

```json
{
  "task": "story_ideas",
  "niche": "{{niche}}",
  "audience": "{{audience}}",
  "language": "{{language}}",
  "core_feeling": "{{feeling}}",
  "count": 7,
  "per_idea": ["title", "hook_first_2_seconds", "core_feeling", "tension", "seeded_clue", "twist", "earned_payoff", "authentic_detail"],
  "rules": ["no repeated territory", "no cartoon villains", "child-safe conflict", "payoff earned by a choice"]
}
```

Territories to rotate: kindness noticed, a small sacrifice, honest mistake and forgiveness, misunderstanding cleared up, quiet hero, lost-and-found, underdog effort, reunion.

**Gate:** stop after seven ideas. Wait for "IDEA N".

## Step 2: Script and beat list

Variables: `{{idea}}`, `{{seconds}}` (default 60), `{{pov}}`

```json
{
  "task": "story_script",
  "idea": "{{idea}}",
  "target_seconds": "{{seconds}}",
  "word_range": "130-200",
  "pov": "{{pov}}",
  "output": ["3_hook_options", "title", "voiceover_block", "numbered_beats"],
  "style": "short sentences, strong verbs, no filler, open loop every two beats",
  "beats": "10 to 12, one clip each, 5 to 8 seconds"
}
```

**Hook rule:** the first spoken line is a feeling or a question, not scene-setting. It is also the first frame's image.

**Gate:** approve the script before any generation. Check that every fact and emotional turn is something a viewer would believe.

## Step 3: Character lock

Variables: `{{name}}`, `{{age}}`, `{{look}}`, `{{outfit}}`, `{{style}}`

```json
{
  "task": "character_prompt",
  "name": "{{name}}",
  "age": "{{age}}",
  "look": "{{look}}",
  "outfit": "{{outfit}}",
  "style": "{{style}}",
  "must_include": ["face shape", "skin tone", "eye shape and color", "hair", "one distinctive feature", "default emotion"],
  "forbidden": ["character sheets", "turnarounds", "text on clothing or props"]
}
```

For PuppyToons stories, Azula and the Baker Family follow [character-bible/azula-and-family.md](character-bible/azula-and-family.md) exactly. Save the approved image and reuse the same text block every time.

## Step 4: Scene images

Variables: `{{beat}}`, `{{cast}}`, `{{action}}`, `{{place}}`, `{{time}}`, `{{shot}}`, `{{mood}}`

```json
{
  "task": "scene_image",
  "beat": "{{beat}}",
  "cast": "{{cast}}",
  "action": "{{action}}",
  "place": "{{place}}",
  "time_of_day": "{{time}}",
  "shot": "{{shot}}",
  "mood": "{{mood}}",
  "suffix": "vertical 9:16, polished 3D family-film animation, soft cinematic light, shallow depth of field, same character identity as the reference, no text, no logos"
}
```

Lighting code: warm gold = safety, cool blue = worry, soft diffused = tenderness, rim light = proud moment, deep shadow = mystery.

**Gate:** every scene image is checked against the character reference before it is animated. A bad image is cheap to redo; a bad clip is a wasted render.

## Step 5: Scene clips (plain text, no JSON)

VideoExpress limits from your v2 workflow apply: up to five clips at a time, up to 10 seconds each, about 30 to 60 seconds to render. Work in batches of five.

Template (one paragraph per clip):

```
{shot} of {character} in {place}, {time of day}. {One continuous action}. Camera: {slow push-in / gentle pan / locked with subtle life}. Face: {expression A} to {expression B}. Pacing: {slow build / gentle / lively}. Ambient sound: {room tone}. Sound effect: {effect and timing}. Voice: {exact line, or "no dialogue, narration added later"}. Duration {5-8} seconds, vertical 9:16, smooth cinematic motion, identity locked to the reference image. Avoid: face morphing, extra limbs, flicker, warping, text overlays.
```

Tool notes:
- **Veo 3:** start from the approved scene image, one action per clip. Quoted dialogue produces spoken audio; if lip-sync drifts, use "no dialogue".
- **Seedance 2.0:** same reference image, state the camera move explicitly, chain clips by using one clip's last frame as the next first frame.
- **Rule:** one action per clip. Two actions means two clips.

## Step 6: Voice and edit

Voice anchor (reuse verbatim): *Warm, natural narrator, medium pace, clear pronunciation, consistent tone and volume in every scene.*

1. Generate narration as its own audio file.
2. Lay narration first and cut any pause longer than half a second.
3. Cut clips to the beats, one clip per beat.
4. Simple cuts or short fades. A slow subtle zoom on still moments.
5. Music bed at 15 to 20 percent of narration volume; ambience and effects underneath.
6. Use only licensed, original, or public-domain audio and note each source.

## Step 7: Publish

- **Title:** curiosity without a spoiler, under 60 characters.
- **Hook:** visible in the first two seconds.
- Follow [youtube/upload-checklist.md](youtube/upload-checklist.md), including the audience designation and the synthetic-content disclosure.
- After publishing, check the 3-second retention mark and adjust the hook style, not the whole system.

## Quality gates

**Gate 1, script:** one feeling, one seeded clue, one earned payoff, no cruelty or shaming, every beat numbered.
**Gate 2, image:** matches the character reference, correct setting, no stray text, nothing scary.
**Gate 3, clip:** one action, identity intact, smooth motion, no extra limbs or duplicates.
**Gate 4, final watch:** full export with sound on, the hook lands in two seconds, narration and picture match, runtime 45 to 90 seconds.

## Worked pilot: "The Drawing on the Fridge"

*Feeling: wanting your effort to be noticed.*

- **Hook:** "Maya drew the same picture four times, and nobody said a word."
- **Tension:** Maya, 4, keeps redrawing Azula for the family fridge, but the house is busy and each drawing gets set aside.
- **Seeded clue:** a small gap on the fridge door, framed by a magnet nobody uses.
- **Twist:** Azula carries each rejected drawing, one by one, to Maya's bedroom wall. The family finds a whole gallery.
- **Earned payoff:** Maya chooses to give her fifth drawing to Leo instead of the fridge, and the family finally notices all of them.
- **Authentic detail:** a crayon with a chewed paper wrapper.
- **Beats:** 10 clips of 5 to 7 seconds, about 60 seconds total.

## Run log

| Date | Idea | Script OK | Images | Clips | Edit | Published | Fix next time |
|------|------|-----------|--------|-------|------|-----------|---------------|
|      |      |           |        |       |      |           |               |

## Sources

- [From Idea to Viral Video: AI Storytelling, The Radio TV](https://theradiotv.net/from-idea-to-viral-video-ai-storytelling/): the workflow order and the idea/visual/motion prompt structure this playbook adapts.
- [PLAYBOOK-v2.md](PLAYBOOK-v2.md): the repo's structure, VideoExpress batch limits, and quality-gate approach.
