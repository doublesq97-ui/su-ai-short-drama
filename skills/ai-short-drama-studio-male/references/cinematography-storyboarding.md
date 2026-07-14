# Cinematography and storyboarding

Use this reference to convert a locked script and approved assets into a tool-neutral shot plan with playable staging, readable information, and continuous screen space.

## Role boundary

The **cinematography / storyboard director** owns shot purpose, staging for camera, framing, screen direction, camera movement, visual rhythm, and the storyboard handoff. The **performance director** owns intention and playable behavior. The **art director** owns the set and prop design. The **sound coordinator** owns audio layering. The storyboard may expose a story, asset, or performance defect, but it must return that defect to the owning role instead of silently rewriting canon.

Tool-specific syntax, parameter values, reference-slot rules, and provider limitations belong only in `tool-adapters.md` or a verified project adapter.

## Define the units before planning

Use these terms consistently:

- **scene**: continuous dramatic action in a defined place and time;
- **shot**: one editorial view with a clear dramatic task;
- **beat**: a change in action, information, emotion, or power inside a scene or shot;
- **generation clip**: one model or production request, which may contain one shot or a limited continuous progression;
- **edit point**: the intended transition between selected material.

A beat is not automatically a cut. Do not confuse a list of timed actions with multiple camera cuts. Do not force a universal number of shots, beats, or seconds.

## Required inputs

Obtain:

- the locked scene or episode script and intended dialogue meaning;
- approved character, look-state, scene, prop, and interface assets;
- entry state from the preceding shot and required exit state for the next;
- format, aspect ratio, delivery length, rating, and accessibility requirements;
- verified production or model capabilities if generation is requested;
- unresolved risks from casting, art, performance, sound, and continuity.

If an asset is only a candidate, label the storyboard provisional and do not present it as locked production instruction.

## Shot-design workflow

### 1. State the dramatic task

Give every shot one primary task:

- establish place, status, relationship, or geography;
- reveal or conceal information;
- show a decision, action, consequence, or reaction;
- change power, distance, risk, resource, or commitment;
- provide a transition, evidence insert, or release.

If a shot has no task, merge it or remove it. If it has several competing tasks, divide them into a coherent sequence.

### 2. Block action before choosing camera movement

Map the scene in simple spatial terms:

- entrances, exits, doors, windows, furniture, hazards, and usable depth;
- each character's start zone, facing direction, eyeline, route, and end zone;
- prop locations, holders, handoffs, and final states;
- contact points, safe distance, and who initiates each interaction;
- foreground, midground, background, and off-screen sources;
- the action axis and intended screen direction.

Do not design a beautiful angle that makes the scripted movement impossible.

### 3. Select framing by information priority

Choose the smallest framing that still communicates the task:

- wide or full views for geography, scale, group relation, and whole-body action;
- medium views for dialogue, gesture, and relation to space;
- close views for decisions, reactions, and precise emotional evidence;
- inserts for a prop, hand, interface, clue, or irreversible action.

Re-establish geography after a major entrance, axis change, crowd movement, impact, or spatially confusing insert. In vertical framing, protect faces, hands, interactive props, and movement destinations from top and bottom crop. Keep important text and captions within the project's verified safe area.

### 4. Choose angle and movement with a reason

Write camera instructions in four parts:

```text
Start frame: [subject, size, position, and visible context]
Movement: [direction and method]
Extent and speed: [small/large, slow/fast, stable/subjective]
End frame: [where attention lands and why]
```

Use a static camera when performance or evidence should dominate. Use a push, pull, pan, tilt, track, follow, rise, fall, handheld impression, or motivated reframing only when the movement reveals, pursues, destabilizes, isolates, or changes relation. Avoid ornamental movement that competes with the dramatic task.

### 5. Budget complexity

Evaluate each generation clip or production setup across:

- number of visible identities and speaking characters;
- contact, fighting, eating, object transfer, vehicles, animals, crowds, or transformation;
- camera movement plus subject movement;
- exact lip sync, overlapping speech, or long dialogue;
- readable text, screens, reflections, mirrors, or transparent surfaces;
- lighting, weather, wardrobe, injury, and state transitions;
- number of beats and intended hard cuts.

For high complexity, choose one or more: improve references, simplify blocking, reduce simultaneous actions, separate the insert, split the clip, move exact text or effects to post, or revise the scene with approval. Never hide production risk behind a longer prompt.

## Spatial and action continuity

### Axis and screen direction

- Establish the action axis for dialogue, travel, pursuit, combat, or exchange.
- Keep eyelines and left/right screen positions consistent while staying on one side of the axis.
- Cross the axis only through a motivated neutral view, visible camera move, character movement that redraws the axis, or a clear re-establishing shot.
- Preserve travel direction across cuts unless reversal is a deliberate story event.
- Record any intentional discontinuity in the handoff.

### Entrances and exits

An exit side implies the next entry direction unless geography shows a change. Record door state, distance traveled, pace, carried objects, and who sees the entrance. Do not let a character appear at a destination without a plausible transition when the travel itself matters.

### Object and contact continuity

Break every transfer or contact action into observable states:

1. **before**: owner, hand, object orientation, distance, and intent;
2. **contact**: who initiates, where contact occurs, and whether it is maintained;
3. **after**: new owner, hand, orientation, body position, reaction, and exit state.

Use this sequence for giving an object, grabbing an arm, opening a door, sitting, drinking, striking, falling, treating an injury, or using a device. Avoid ambiguous pronouns; name the actor, target, body area, object, and direction.

### Action and combat geography

- Establish participants, obstacles, exits, objective, and relative distance before rapid coverage.
- Preserve cause and effect: preparation, action, impact or avoidance, reaction, and changed state.
- Use inserts and reaction shots to clarify a decisive event, not to conceal incoherent geography.
- Track weapons, ammunition, powers, wounds, debris, and environmental damage through the continuity ledger.
- Favor readable force and consequence over graphic injury. Use silhouette, obstruction, sound, off-screen action, aftermath, and reaction where direct depiction would be unsafe, excessive, or unnecessary.

Non-graphic framing is a creative and rating decision, not a technique for disguising prohibited content or bypassing a provider's safeguards.

## Dialogue, reaction, and timing

- Time dialogue by reading it aloud at the intended performance pace. Include breath, interruption, reaction, movement, and edit space.
- Do not use a universal characters-per-second rule as a substitute for a read-through.
- Preserve the first meaningful reaction after an important line or event.
- Let a line continue across a cut only when speaker identity, lip-sync strategy, and sound continuity are clear.
- Separate production audio from OS, score, stylized effects, captions, and replacement dialogue in the handoff.
- If the selected tool cannot reliably perform the dialogue, create clean visual coverage and assign voice and lip-sync work to a verified downstream process.

## Text, interfaces, and evidence

Exact wording on phones, documents, signs, messages, subtitles, diagrams, logos, or dashboards is a high-risk production task. Plan:

1. a stable, clean insert with adequate dwell time;
2. a legible composition and interaction without depending on generated text accuracy;
3. exact text, UI, captions, or licensed branding in post unless a verified method can reproduce it;
4. reaction and story consequence after the insert.

Do not include unlicensed logos, private data, or documents merely because they appeared in a reference image.

## Tool-neutral shot record

For each shot, provide:

```markdown
### [Shot ID] · [dramatic task]
- Source scene and beat:
- Suggested duration and rationale:
- Entry continuity:
- Exit continuity:
- Characters, scene, props, and locked versions:
- Blocking and action chain:
- Start frame:
- Camera movement, extent, and speed:
- End frame:
- Performance focus:
- Production sound:
- Post tasks:
- Complexity risks and fallback split:
```

Derive any provider prompt from this record. The shot record remains authoritative when tools change.

## Storyboard-to-production handoff

Deliver:

- ordered shot IDs and edit intent;
- a simple floor plan or spatial description for complex scenes;
- entry/exit continuity and action-state ledger;
- approved asset IDs and versions only;
- duration rationale and dialogue read-through result;
- sound, exact text, VFX, captions, and post assignments;
- generation or production risks with fallback coverage;
- tool adapter and verification date when a specific tool is used.

## Acceptance gate

Do not lock the storyboard until:

- every shot has one readable dramatic task;
- spatial geography, axis, eyelines, entrances, exits, contact, and prop transfers are coherent;
- timing is supported by a read-through or test rather than a fixed quota;
- high-risk actions have a practical split or fallback;
- exact text and stylized audio have an assigned production route;
- all referenced assets are approved and rights-cleared for the intended use;
- tool-neutral decisions are separated from provider-specific syntax.
