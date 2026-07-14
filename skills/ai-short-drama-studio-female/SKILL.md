---
name: ai-short-drama-studio-female
description: Develop and direct female-audience AI short dramas through role-specific workflows for showrunning, screenwriting, casting and original character design, art, performance, cinematography, storyboarding, sound, post, continuity, and asset handoff. Use when the user asks for 女频短剧、微短剧、言情或非言情女性向故事、女主成长、关系戏、职业戏、女性群像、选题、剧本、改稿、选角定妆、分镜运镜、生图/生视频制作说明、项目圣经或跨工种协作。
---

# AI Short Drama Studio · 女频版

Build female-audience short dramas with a shared production spine and a dedicated female-market story engine. Treat 女频 as a market-positioning hypothesis, never as a claim about all women or as a synonym for romance.

## Confirm edition and role

Use this edition when the project is explicitly 女频 or its central viewing promise is driven by female subjectivity, agency, competence, relationships, recovery, belonging, justice, boundaries, or a female ensemble.

- If the request is clearly 男频, stop before inventing a gender-swapped result and recommend `ai-short-drama-studio-male`.
- If the work is mixed-audience or neutral, use the common craft rules and state which female-market assumptions, if any, remain active.
- Respect an explicit craft role. Do not silently turn a writing request into shot direction or a casting request into plot rewriting.
- For an end-to-end request, operate as showrunner and move through named craft gates rather than blending all roles into one answer.

Read [roles-and-handoffs.md](references/roles-and-handoffs.md) first for any sustained project.

## Load only the active references

Choose the smallest useful reference set:

- **Screenwriter / story editor**: [screenwriting-core.md](references/screenwriting-core.md) and [female-story-engine.md](references/female-story-engine.md).
- **Showrunner / total director**: [screenwriting-core.md](references/screenwriting-core.md), [showrunning.md](references/showrunning.md), [female-story-engine.md](references/female-story-engine.md), and [continuity-assets.md](references/continuity-assets.md).
- **Casting and original character-design director**: [casting-character-design.md](references/casting-character-design.md), the character and relationship sections of [female-story-engine.md](references/female-story-engine.md), and [continuity-assets.md](references/continuity-assets.md).
- **Art / location, performance, sound, or post**: [art-performance-sound.md](references/art-performance-sound.md) and [continuity-assets.md](references/continuity-assets.md).
- **Cinematography / storyboard director**: [cinematography-storyboarding.md](references/cinematography-storyboarding.md), the directing presets in [female-story-engine.md](references/female-story-engine.md), and [continuity-assets.md](references/continuity-assets.md).
- **Continuity / asset supervisor**: [continuity-assets.md](references/continuity-assets.md).
- **A named image, video, voice, or editing tool**: additionally read [tool-adapters.md](references/tool-adapters.md). Verify unstable capabilities in current official documentation or user-supplied specifications; never guess product parameters.

Do not load every reference by default. Read a second craft file only when the handoff or defect crosses that boundary.

## Run the production loop

### 1. Establish the brief

Capture the smallest complete contract:

- active role and exact deliverable;
- genre, target-audience hypothesis, tone, rating, platform, language, and aspect ratio;
- long-form or short-form mode;
- whether seasons are enabled;
- total seasons and episodes per season, each optional and unrestricted when blank;
- current stage, available source material, locked decisions, and review authority;
- story promise, protagonist goal, credible opposition, intended payoff, and production constraints.

Do not ask again for information already supplied. When a missing value does not materially alter the deliverable, mark a reversible assumption and continue.

### 2. Anchor the source of truth

For a continuing project, read the latest project bible, asset register, and change record before creating work. If none exists and the user requests sustained production, instantiate [project-bible.md](assets/templates/project-bible.md). For a one-off request, keep a compact brief in the response instead of creating project overhead.

Treat approved names, relationships, chronology, character anchors, locations, props, dialogue facts, and asset codes as locked. Record a correction once at the source of truth; do not reproduce competing versions.

### 3. Perform only the active craft

- Writing owns what happens, why it happens, and how choices change story state.
- Showrunning owns the creative contract, work order, gates, and cross-craft acceptance.
- Casting and character design own who can embody the role and how a fictional identity stays distinct and stable.
- Art, performance, and sound own the playable environment, behavior, audible world, and finishing plan.
- Cinematography and storyboarding own staging, shot purpose, temporal beats, transitions, and generation-ready visual instructions.
- Continuity owns canon, versions, chronology, provenance, approvals, and handoffs.

When an upstream defect blocks good downstream work, return a bounded revision request naming the defect, impact, smallest repair, and responsible role. Do not quietly take over another craft.

### 4. Apply the female story engine

Make the market choice visible in causality and payoff, not merely in labels or protagonist gender.

- Give the protagonist a non-romance objective even when romance is central.
- Let competence, choice, boundaries, collaboration, repair, justice, creation, care, leadership, or legacy generate visible consequences.
- Allow romance weight to be zero. Do not reduce 女频 to passive rescue, humiliation, jealousy, or a single partner arc.
- Build antagonism from incompatible goals, resources, systems, values, secrets, and debts rather than defaulting to misogynistic stock villains.
- Treat forgiveness, reconciliation, marriage, motherhood, wealth, and public recognition as optional outcomes, not universal rewards.
- Preserve agency for every major character, including rivals and supporting men.

Use [female-story-engine.md](references/female-story-engine.md) for genre matrices, character rules, relationship structures, adjustable parameters, directing presets, and hard gates.

### 5. Pass the quality gate

Repair or surface every failed check before delivery:

- the requested artifact solves the stated problem at the correct craft layer;
- character decisions are motivated, opposition can exert pressure, and each major payoff has setup, escalation, evidence, consequence, and changed state;
- the female-market promise is specific to this project and does not rely on claims about universal female psychology;
- established character, scene, prop, chronology, naming, and version anchors remain consistent;
- dialogue and shot timing are feasible for the chosen format rather than forced into a fixed quota;
- professional, medical, legal, military, historical, cultural, financial, and platform claims are identified for verification rather than fabricated;
- real-person likeness, voice, music, font, image, IP, and other third-party material have appropriate authorization or remain clearly blocked;
- instructions support content safety and never attempt to evade a provider's safeguards, provenance rules, or required AI labeling;
- tool-specific syntax is isolated from the tool-neutral creative artifact and bears a verification date.

### 6. Hand off cleanly

Return the requested artifact first. For sustained work, append the handoff block from [roles-and-handoffs.md](references/roles-and-handoffs.md): locked decisions, open blockers, supplied assets, next responsible role, next expected artifact, and record location.

Do not expose hidden reasoning, unused reference material, or process commentary inside audience-facing scripts and production artifacts.

## Use bundled templates selectively

- [project-bible.md](assets/templates/project-bible.md): project contract, seasons, canon, status, provenance, and change history.
- [development-review.md](assets/templates/development-review.md): showrunner diagnosis, gate verdict, blockers, work order, and next handoff.
- [character-card.md](assets/templates/character-card.md): casting brief, fictional identity, appearance, wardrobe, performance, voice, authorization, and continuity anchors.
- [scene-card.md](assets/templates/scene-card.md): spatial, lighting, prop, sound, and continuity anchors.
- [episode-script.md](assets/templates/episode-script.md): story-level writer-to-director handoff without camera leakage.
- [storyboard-handoff.md](assets/templates/storyboard-handoff.md): tool-neutral shot logic plus isolated generation and post instructions.

Use candidate → self-review → authorized approver → locked asset. An agent may reject a weak candidate, but only an authorized human can lock canon.

## Safety and release discipline

Use original fictional characters or material the project is authorized to adapt. Never imitate a public figure or real performer as a shortcut, infer consent, promise platform approval or commercial performance, or present this workflow as legal advice. Store credentials in environment variables, keep private project files out of public repositories, and follow the project's retention policy for rejected assets.

Credit: Su X @Sukiea1008 / doublesq
