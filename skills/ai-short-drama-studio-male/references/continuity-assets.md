# Continuity and asset supervision

Use this reference to keep story canon, character and scene states, files, versions, rights, and production handoffs consistent across sessions and tools.

## Role boundary

The **continuity / asset supervisor** records approved facts and detects mismatches. This role does not invent approval, choose a favorite candidate, or rewrite story and design decisions. When two sources conflict, identify the conflict, preserve both records, and route the decision to the owning role and `authorized_approver`.

The project bible is the source of truth for locked canon. Tool workspaces, chat history, filenames, and generated galleries are evidence or working material, not automatic canon.

## Status model

Use one status consistently:

- `proposal`: editable concept or asset candidate;
- `selected`: preferred, awaiting required verification or approval;
- `locked`: exact version approved by the authorized approver;
- `in-production`: work currently derived from a locked input;
- `rejected`: not selected and never canonical;
- `superseded`: previously locked, replaced by a later approved version;
- `blocked`: missing a named decision, right, fact, or dependency.

Never call a generated output final merely because the tool completed successfully.

## Stable IDs and versions

Use readable, non-ambiguous IDs independent of any provider syntax. Examples:

```text
char-001
char-001-look-002
scene-014
scene-014-state-night-rain
prop-021
shot-e03-017
audio-e03-017-dialogue-v02
```

Provider aliases such as mention tags or asset slots belong in the adapter record, not in the canonical ID.

Increment versions instead of overwriting approved files. A filename should communicate project, asset ID, state, version, and status without depending on character-name punctuation. Keep display names in metadata.

## Minimum asset record

Record:

| Field | Requirement |
|---|---|
| Canonical ID | Stable, provider-neutral identifier |
| Display name and type | Character, look, scene, prop, voice, shot, take, audio, text, or document |
| Version and status | Exact revision and lifecycle state |
| File or resource location | Resolvable path or authorized resource ID |
| Purpose | What the asset controls and what it does not control |
| Source | Original, commissioned, licensed, user-supplied, or generated |
| Rights / consent | Scope, owner or consenting party, restrictions, expiry, attribution |
| Creation record | Creator or tool, model/version if applicable, date, and prompt/brief version |
| Approval record | Authorized approver, date, decision, and notes |
| Relationships | Derived from, supersedes, used by, and dependent assets |
| Integrity | Optional hash, dimensions, duration, MIME type, and color/audio metadata |

The record supports traceability; it does not itself prove legal ownership.

## Candidate-to-lock lifecycle

### 1. Intake

Assign candidate IDs, preserve the supplied source, inspect file type and metadata, and record rights or consent status. Do not upload sensitive or unauthorized material merely to test a tool.

### 2. Candidate production

Store bounded candidates separately from locked assets. Record the brief or prompt version and the tool or human source. Do not allow an alternative candidate to inherit a locked ID.

### 3. Self-review

The responsible craft rejects candidates with identity, anatomy, spatial, performance, sound, text, rights, safety, or technical defects. Record a concise reason. Self-review may narrow the set but cannot lock it.

### 4. Authorized approval

The `authorized_approver` confirms the exact candidate and intended use. A general preference such as “the second direction” is not enough if multiple files could match; resolve it to a candidate ID and version.

### 5. Lock

Create the locked record without deleting or overwriting the source candidate. Update the project bible, downstream alias map, and dependency register. Only the locked version may be treated as canonical.

### 6. Propagation

Every storyboard, prompt, generation job, edit, or release must reference the canonical ID and version. If a downstream tool creates a new derivative, register the derivative and its source relationship.

### 7. Supersession

Changing a locked asset requires a new approved version, a reason, an impact check, and a list of downstream materials to update. Mark the old version `superseded`; do not silently replace it.

### 8. Retention

Apply the project's retention policy to rejected candidates. Consider privacy, consent, license, storage cost, security, and future audit value. It may be appropriate to retain the file, retain only a hash and rejection reason, or delete it after an approved period. Never claim that keeping every rejected image creates legal proof.

## Continuity ledger

For every shot, record both incoming and outgoing state.

### Story and time

- story date and time, elapsed time, season, weather, and location state;
- facts known by each character, promises, secrets, injuries, resources, and unresolved actions;
- setup and payoff status.

### Character state

- location zone, screen side, facing direction, eyeline, posture, and movement vector;
- emotional strategy and level of tension, fatigue, intoxication, illness, or concealment;
- locked look version, wardrobe layers, fastenings, shoes, hair, makeup, dirt, wetness, bloodless injury indicators, and carried items;
- hand occupancy and contact with another character or object;
- dialogue or voice take when continuity depends on timing or vocal state.

### Scene and prop state

- doors, windows, curtains, lights, screens, vehicles, furniture, and environmental damage;
- prop owner, hand, orientation, quantity, contents, open/closed or intact/damaged state, and last visible position;
- food, drink, smoke, candles, weather, water, debris, or other changing elements;
- crowd size, density, direction, and background action.

### Camera and sound continuity

- action axis, screen direction, lens or framing impression when matching matters;
- entry and exit frame, camera height and movement endpoint;
- room tone, ambience, sustained effects, music overlap, OS, and dialogue continuation;
- intended edit point, transition, and handle requirements.

## Spatial continuity procedure

For any scene with movement, contact, pursuit, combat, or multiple entrances:

1. assign simple zones to the scene map;
2. record each character's start zone, route, and end zone;
3. establish the action axis and screen direction;
4. record all door and obstacle states;
5. decompose object transfer or contact into before, contact, and after;
6. verify that the next shot begins from the previous outgoing state;
7. re-establish geography after a deliberate axis change or major displacement.

Flag a mismatch before generation or editing. Do not repair it by changing an unrelated locked asset.

## Alias and tool mapping

Maintain a separate mapping when a provider requires its own IDs:

| Canonical ID + version | Provider / workspace | Provider alias or slot | Verified date | Notes |
|---|---|---|---|---|
| [fill] | [fill] | [fill] | [YYYY-MM-DD] | [responsibility / limits] |

Removing or changing a provider alias must not change the canonical asset identity.

## Rights, consent, and data handling

- Record authorization for real-person likeness, body, performance, and voice references before use.
- Reject recognizable public-figure replicas outright; stylization, feature mixing, or indirect naming does not make them acceptable. Use a private person's identity only within an explicitly authorized and consented scope.
- Keep consent records and private source files out of public prompts, repositories, and deliverables unless publication is explicitly authorized.
- Record licenses and attribution requirements for images, fonts, music, sound, footage, logos, documents, and datasets.
- Do not store API keys, session cookies, signed URLs, passwords, personal contact data, or other secrets in project files.
- Check downloadable URLs before archiving; generated-resource links may expire.
- Verify MIME type, dimensions, duration, and basic integrity rather than trusting the extension alone.
- Follow deletion, revocation, and access restrictions in the applicable consent or license.

If rights are unclear, mark the asset `blocked` and substitute an original, cleared reference. Do not infer permission from online availability.

## Handoff and release procedure

Before each craft handoff:

1. identify the locked input IDs and versions;
2. list new proposals separately from canon;
3. provide incoming and outgoing continuity states;
4. list missing rights, facts, assets, or approvals;
5. name the next role and expected artifact;
6. update the project bible and change log.

Before release, reconcile the actual selected takes and final audio/text with the project bible. Archive the released version, source locations, license/consent records, required attributions, and superseded dependencies according to project policy.

## Validation checklist

- [ ] Every referenced asset resolves to one canonical ID and exact version.
- [ ] No candidate is mislabeled as locked.
- [ ] The authorized approver and approval date are recorded.
- [ ] Real-person likeness and voice references have an explicit permitted scope.
- [ ] Entry/exit states match across adjacent shots.
- [ ] Screen direction, eyelines, contacts, and prop transfers are coherent.
- [ ] Wardrobe, hair, makeup, injury, dirt, wetness, weather, light, and damage states match story time.
- [ ] Provider aliases are separated from canonical IDs.
- [ ] Rejected and superseded material follows the retention policy.
- [ ] No secret or private record is exposed in public artifacts.
- [ ] The project bible describes the released work rather than an obsolete plan.
