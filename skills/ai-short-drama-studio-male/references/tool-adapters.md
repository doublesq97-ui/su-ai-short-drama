# Tool adapters

`last_verified: 2026-07-14`

Use this reference only after the creative decision and tool-neutral production record are complete. It defines how to verify and document a current image, video, audio, voice, or post-production tool without leaking temporary product behavior into the common directing rules.

This file intentionally contains no fixed provider model IDs, endpoint paths, duration ranges, reference limits, or payload fields. Those details change. Verify them in current official documentation before use.

## Non-negotiable rule

If a parameter, capability, limit, policy, or commercial right is unknown, inspect the provider's official documentation or ask the user. Never guess. Never copy an unverified value from an old project, blog post, screenshot, community prompt, or model memory.

Record the official source URL, verification date, product or model version, region, and account context. If official documentation is unavailable or contradictory, mark the capability `unknown` or `blocked` and use a safer fallback.

## Separation of layers

Maintain three distinct artifacts:

1. **Creative record**: dramatic task, blocking, framing, performance, sound, continuity, and approved assets.
2. **Capability profile**: what the current tool is officially documented and locally tested to support.
3. **Invocation adapter**: the exact syntax, parameters, file preparation, polling, and output handling for that verified tool version.

The creative record remains authoritative when an adapter changes. Do not put provider aliases, model IDs, or API payloads into canonical character, scene, or shot IDs.

## Capability-verification checklist

Before writing an adapter, verify from official documentation:

- provider, product, model or feature name, exact version, and availability region;
- accepted input modes: text, image, video, audio, masks, keyframes, or references;
- supported formats, codecs, MIME types, dimensions, aspect ratios, resolutions, durations, and file-size limits;
- number and semantic role of references, including whether identity, style, scene, first frame, last frame, or editing inputs can coexist;
- prompt or instruction limits and whether a dedicated negative field exists;
- seed, variation, edit, extension, continuation, camera, lip-sync, dialogue, music, or sound controls;
- synchronous or asynchronous execution, task states, polling guidance, timeout, cancellation, retry, and rate limits;
- output format, metadata, watermark behavior, URL expiry, storage, privacy, training-use, and deletion controls;
- safety restrictions, likeness and voice rules, content labeling, age restrictions, and prohibited uses;
- commercial-use terms, ownership language, attribution, and account-plan restrictions;
- pricing unit and any quality, duration, or audio multiplier relevant to the production decision.

Do not infer support because a parameter name seems plausible. Do not claim one provider's prompt or payload works in another.

## Adapter record

Create or update a project-specific record:

```markdown
# Adapter · [provider / product / model]

- Status: [verified / partially verified / unknown / blocked]
- Verified on: [YYYY-MM-DD]
- Official documentation: [direct URL]
- Region / account context: [fill]
- Intended task: [image identity / scene reference / video / audio / voice / edit / post]
- Supported inputs: [verified only]
- Supported outputs: [verified only]
- Bounds and incompatibilities: [verified only]
- Safety / likeness / voice constraints: [verified only]
- Commercial / retention notes: [verified only; seek professional review when needed]
- Canonical-to-provider alias map: [path]
- Test fixture and result: [path or summary]
- Fallback: [fill]
```

Place exact invocation syntax under a clearly dated section. Do not present a stale adapter as current.

## Tool-neutral prompt mapping

Adapt from positive, observable production decisions:

- approved subject identity and look state;
- approved scene geography and state;
- shot task, start frame, movement, extent, speed, and end frame;
- ordered action and performance beats;
- production sound requested from this tool, if verified;
- exact exclusions needed for this shot and supported by the tool;
- output format required by the edit.

Keep negative instructions short and specific. Solve persistent problems at the source—asset, staging, tool choice, or post—rather than accumulating a universal negative list.

Explicitly state each reference's responsibility when the tool supports multiple references. For example, one may control original character identity, another scene layout, and another first-frame composition. Do not assume the tool honors this separation; verify with a bounded test.

## Image-generation adapter procedure

1. Confirm whether the task is original generation, editing, variation, outpainting, or reference-guided design.
2. Verify supported sizes, formats, reference types, masks, and edit semantics.
3. Prepare only rights-cleared inputs and strip secrets or unnecessary personal metadata.
4. Generate bounded candidates into the candidate area.
5. Inspect identity, anatomy, expression, hands, wardrobe, scene, text, watermark, and downstream suitability.
6. Record tool/model version, brief or prompt version, output metadata, and defects.
7. Send surviving candidates through self-review and `authorized_approver`; do not auto-lock.

If the provider disallows a reference or use, do not stylize, rename, crop, redraw, or transform it to evade that restriction. Create an original cleared direction or use an allowed workflow.

## Video-generation adapter procedure

1. Map the tool-neutral shot record to one feasible generation clip.
2. Verify duration, aspect ratio, resolution, reference compatibility, camera controls, audio behavior, first/last-frame behavior, continuation, and output handles.
3. Reduce action complexity to the verified capability budget; split geography, contact, text, or dialogue when necessary.
4. Assign exact text, captions, logos, UI, OS, music, or dialogue replacement to post unless the verified workflow can produce them reliably and lawfully.
5. Test one representative high-risk shot before converting an episode.
6. Store returned task IDs, selected output, failure state, and expiring resource URL securely.
7. Review identity, space, action order, timing, continuity, sound, and policy compliance before take selection.

Do not hard-code a universal clip duration, dialogue window, number of characters, beat count, cut count, or aspect ratio. Set them from story needs and verified capability.

## Audio and voice adapter procedure

1. Identify whether the task is original synthetic voice, authorized voice clone, speech editing, dialogue replacement, ambience, Foley, effects, music, or mastering.
2. Verify accepted languages, voice controls, consent requirements, watermark or disclosure rules, output format, sample rate, duration, and commercial terms.
3. Use a generic original voice profile unless a private person has explicitly authorized and consented to the intended synthetic use.
4. Do not target a public figure, celebrity, politician, performer, or creator through name, sample, indirect descriptor, stylization, feature mixing, or imitation request. This workflow does not support recognizable public-figure replicas.
5. Test pronunciation, emotional range, timing, breath, artifacts, and consistency across scenes.
6. Store clean source, processed version, cue timing, voice version, authorization status, and replacement history separately.

If consent scope does not explicitly allow synthetic derivatives or cloning, treat it as not allowed.

## Editing and post adapter procedure

Verify project format, frame rate, resolution, color handling, audio layout, caption format, font and music licenses, export codec, and delivery requirements. Keep exact text and captions editable. Preserve handles and source versions. Do not bake a provisional watermark, subtitle, logo, or temp track into the only master.

## Security and privacy

- Put API keys and tokens in environment variables, the provider's secret store, or an approved credential manager.
- Never write secrets into Markdown, source control, prompts, screenshots, logs, or project-bible fields.
- Redact signed URLs, session cookies, private endpoints, contact information, and consent documents from public artifacts.
- Use least-privilege credentials and an authorized workspace.
- Confirm whether uploads may be retained or used for training before sending confidential scripts, real-person references, or unreleased assets.
- Download expiring outputs to an authorized project location and verify MIME type, integrity, dimensions, and duration.
- Do not publish third-party source assets with the open-source Skill unless redistribution rights are explicit.

## Safety and rights

- Follow the provider's current safeguards and prohibited-use rules.
- Do not rewrite, obfuscate, translate, stylize, or relabel content to evade moderation or reference restrictions.
- Use original or rights-cleared character, scene, voice, music, footage, and graphic references.
- Treat public online availability as neither consent nor license.
- Use non-graphic framing, off-screen implication, reaction, and aftermath when appropriate to story and rating; do not use them to conceal a prohibited request.
- Record required labels, disclosures, attribution, or provenance metadata in the release plan.

## Verification test

Before production-scale use, run a small representative test that checks:

- identity and scene-reference behavior;
- temporal action order and camera instruction adherence;
- spatial, prop, wardrobe, and lighting continuity;
- dialogue, lip-sync, ambience, or silence behavior if requested;
- exact-text and watermark behavior;
- output metadata, URL expiry, and file integrity;
- safety, consent, license, and account-plan compatibility;
- cost and turnaround sufficient for the intended batch.

Record observed behavior separately from official capability. A successful test is evidence for that configuration, not a permanent universal rule.

## Failure and fallback rules

- **Invalid parameter or model**: re-check current official documentation; do not try guessed alternatives in production.
- **Unsupported input combination**: separate the task or choose a verified workflow.
- **Identity or space drift**: strengthen the approved reference set, simplify the shot, or change tools; do not add unauthorized likeness references.
- **Unreadable text**: create a clean plate and composite verified text in post.
- **Unstable dialogue or audio**: generate clean visuals and use an authorized voice/post workflow.
- **Policy rejection**: stop and follow the provider's guidance; do not attempt semantic disguises or alternate encodings.
- **Unclear rights or consent**: mark the asset blocked and replace it with an original cleared alternative.
- **Documentation unavailable**: keep the adapter unknown, disclose the limitation, and ask before proceeding.

## Adapter acceptance gate

Do not mark an adapter `verified` until:

- every production-critical claim has a current official source;
- a representative test matches the documented behavior;
- unknown or account-specific limits are explicit;
- secrets and private data are excluded from artifacts;
- likeness, voice, source, safety, and commercial constraints are recorded;
- the fallback path is practical;
- the verification date is current for the production decision.
