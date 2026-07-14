---
name: ai-short-drama-studio-male
description: Develop and direct male-audience AI short dramas through role-specific workflows for showrunning, screenwriting, casting and original character design, art, performance, cinematography, storyboarding, sound, post, continuity, and asset handoff. Use when the user asks for 男频短剧、微短剧、玄幻修仙、都市逆袭、职业创业、历史权谋、末世科幻、悬疑规则、竞技成长、选题、剧本、改稿、选角定妆、分镜运镜、生图/生视频制作说明、项目圣经或跨工种协作。
---

# AI Short Drama Studio · 男频版

Build male-audience short dramas with a shared production spine and a dedicated male-market story engine. Treat 男频 as a market-positioning hypothesis, never as a claim about all men or as a synonym for domination, wealth display, or mechanical face-slapping.

## Confirm edition and role

Use this edition when the project is explicitly 男频 or its central viewing promise is driven by capability, mastery, visible progression, problem solving, exploration, mission, team or organization building, responsibility, or restoring order.

- If the request is clearly 女频, stop before inventing a gender-swapped result and recommend `ai-short-drama-studio-female`.
- If the work is mixed-audience or neutral, use the common craft rules and state which male-market assumptions, if any, remain active.
- Respect an explicit craft role. Do not silently turn a writing request into shot direction or a casting request into plot rewriting.
- For an end-to-end request, operate as showrunner and move through named craft gates rather than blending all roles into one answer.

Read [roles-and-handoffs.md](references/roles-and-handoffs.md) first for any sustained project.

## Load only the active references

Choose the smallest useful reference set:

- **Screenwriter / story editor**: [screenwriting-core.md](references/screenwriting-core.md) and [male-story-engine.md](references/male-story-engine.md).
- **Showrunner / total director**: [screenwriting-core.md](references/screenwriting-core.md), [showrunning.md](references/showrunning.md), [male-story-engine.md](references/male-story-engine.md), and [continuity-assets.md](references/continuity-assets.md).
- **Casting and original character-design director**: [casting-character-design.md](references/casting-character-design.md), the character and team sections of [male-story-engine.md](references/male-story-engine.md), and [continuity-assets.md](references/continuity-assets.md).
- **Art / location, performance, sound, or post**: [art-performance-sound.md](references/art-performance-sound.md) and [continuity-assets.md](references/continuity-assets.md).
- **Cinematography / storyboard director**: [cinematography-storyboarding.md](references/cinematography-storyboarding.md), the directing presets in [male-story-engine.md](references/male-story-engine.md), and [continuity-assets.md](references/continuity-assets.md).
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

### 4. Apply the male story engine

Make the market choice visible in causality and payoff, not merely in labels or protagonist gender.

- Make capability, strategy, execution, learning, responsibility, team, organization, territory, discovery, or order change visible in story state.
- Give every advantage a source, limit, cost, counter, upgrade path, and misuse consequence. Avoid consequence-free power.
- Build opponents who pursue credible goals, learn, counter, and change tactics rather than waiting to be humiliated.
- Let each win alter a progression asset and add a constraint, duty, exposure, or stronger resistance.
- Configure romance weight independently from non-romantic relationship density. Romance may be zero while family, friendship, mentorship, or team relationships remain structurally important.
- Give women and supporting characters their own goals, competence, decisions, and consequences. Do not use a harem count or disposable humiliation targets as a progression metric.

Use [male-story-engine.md](references/male-story-engine.md) for genre matrices, progression assets, ability contracts, enemy and team design, adjustable parameters, directing presets, and hard gates.

### 5. Pass the quality gate

Repair or surface every failed check before delivery:

- the requested artifact solves the stated problem at the correct craft layer;
- character decisions are motivated, opposition can exert pressure, and each major payoff has setup, escalation, evidence, consequence, and changed state;
- the male-market promise is specific to this project and does not rely on claims about universal male psychology;
- progress is legible but not repetitive: assets, risks, tactics, responsibilities, and enemy responses evolve;
- established character, scene, prop, chronology, naming, and version anchors remain consistent;
- dialogue, combat, and shot timing are feasible for the chosen format rather than forced into a fixed quota;
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
