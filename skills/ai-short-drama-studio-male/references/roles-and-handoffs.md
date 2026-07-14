# Roles and handoffs

Use this reference to select one active craft, preserve upstream decisions, and make the next handoff executable.

## Role map

| Role | Owns | Required inputs | Standard output | Boundary |
|---|---|---|---|---|
| Showrunner / total director | Creative contract, production sequence, quality gates, cross-craft decisions | User goal, story material, project bible if present | Production brief, lock list, work order, acceptance decision | Do not absorb every craft into one vague response |
| Screenwriter / story editor | Premise, character choices, conflict, scenes, dialogue, hooks, setup and payoff | Brief, audience branch, established canon | Diagnosis, outline, episode script, revision memo | Stop at what happens and why; leave shot execution to directing |
| Casting and character-design director | Casting brief, original character identity, look system, wardrobe states, performance anchors | Locked role function, arc, tone, production constraints | Character-card candidates and locked card | Do not use celebrity likeness as a shortcut or change the character arc |
| Art / location director | Space, period, materials, props, palette, location continuity | Locked scenes, action needs, visual direction | Scene cards, prop register, visual states | Design spaces that support action; do not rewrite scenes to fit a pretty image |
| Performance director | Intention, playable action, reaction, blocking logic, emotional transitions | Locked scene and character behavior anchors | Performance beat sheet and actor / generation guidance | Direct behavior, not camera placement |
| Cinematography / storyboard director | Shot purpose, staging, framing, movement, temporal beats, visual continuity | Locked script, approved character and scene assets | Shot plan, storyboard handoff, generation-ready instruction blocks | Preserve story facts and dialogue intent; return structural defects upstream |
| Sound and post coordinator | Dialogue strategy, production sound, ambience, OS, music, effects, edit rhythm, captions | Locked storyboard or rough cut plan | Sound-layer plan and post handoff | Separate what must be generated on set/model side from what belongs in post |
| Continuity / asset supervisor | Canon, codes, versions, chronology, rights/source fields, status and handoff records | All confirmed decisions and assets | Updated project bible, mismatch report, version register | Record decisions; never invent missing approvals |

## Role selection rules

- Honor an explicit role request even when another role could add value. Offer a handoff after completing the requested craft.
- Combine roles only when the user asks for an end-to-end pass or the project is deliberately one-person production. Label each role transition and keep its deliverable separate.
- Return work upstream when the current craft cannot repair it without changing intent. State the defect, its impact, the smallest requested revision, and who owns it.
- Treat approval by the project's authorized reviewer as the lock condition. Agent self-review may reject a weak candidate, but it cannot silently convert a proposal into locked canon.

## Status vocabulary

Use one of these states so every role reads the same project:

- **proposal**: a candidate open to structural change;
- **selected**: preferred direction, still awaiting final verification or assets;
- **locked**: user-approved source of truth;
- **in production**: currently being executed against a locked input;
- **superseded**: retained for history but no longer authoritative;
- **blocked**: cannot proceed without a named decision or input.

Do not use “final” for a candidate that has not passed the relevant acceptance gate.

## Handoff contract

End sustained-project work with this compact block:

```markdown
## Handoff

- Audience profile: [male edition / neutral or mixed, with active male-market promises named]
- Completed role: [role]
- Artifact and status: [path or section · proposal/selected/locked]
- Locked decisions: [only confirmed decisions]
- Open blockers: [none, or specific decisions]
- Assets supplied: [asset codes, versions, and locations]
- Next role: [role]
- Next expected output: [one concrete artifact]
- Record update: [project-bible section or “not required for one-off work”]
```

Omit empty operational detail. The next role must be able to start without rereading the entire conversation.

## Acceptance gates

### Writer to showrunner

- Scene objectives, character choices, causal turns, dialogue intent, and episode-end state are explicit.
- Canon conflicts and unresolved story decisions are surfaced.
- The script contains no camera prescription disguised as story action.

### Showrunner to casting / art

- Role function, age range, life experience, tone, time period, and production constraints are stable enough to design against.
- Required character and location states are enumerated.

### Casting / art to storyboard

- The user has locked the character and scene version or explicitly authorized a provisional test.
- Asset codes, anchor descriptions, and usage rights/source status are present.
- Alternative candidates are not mixed into the locked card.

### Storyboard to generation / production

- Each shot has one dramatic task and a coherent action chain.
- Entry and exit continuity are recorded.
- Dialogue or sound timing is feasible for the selected duration.
- Tool-specific syntax is isolated from the tool-neutral shot design.

### Generation / production to post

- Selected takes are identified; rejected takes are not treated as canon.
- Missing inserts, continuity errors, dialogue replacement, captions, music, and effects are listed.
- File names and versions sort into the intended sequence.

### Post to archive

- The delivered cut, source assets, licenses/permissions, prompts or production notes, and change log have stable locations.
- The project bible reflects the actual released version rather than an earlier plan.
