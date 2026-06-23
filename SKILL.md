---
name: ai-video-preproduction-workflow
description: Plan controllable AI video generation workflows before prompting a model. Use when Codex needs to turn a concept, brief, ad, short-film idea, UGC script, dialogue scene, action clip, or product video into a reusable preproduction package covering concept selection, Plan Demo, character boards, scene layout, camera blocking, storyboards, packaging boards, continuity constraints, and final prompt assembly.
---

# AI Video Preproduction Workflow

Use this skill to convert a rough video idea into a structured preproduction package that makes model output more stable, editable, and reusable.

## Core Workflow

1. Define the video goal.
Determine format, duration, aspect ratio, platform, hook, conflict, payoff, and output style before writing generation prompts.

2. Write a Plan Demo.
Lock the story logic first. Specify characters, world rules, timeline beats, camera intent, and continuity risks in prose before creating visual assets.

3. Build the asset chain in order.
Create assets in this sequence unless the user already provides some of them:
- character board
- scene layout
- camera blocking map
- storyboard
- package board
- final video prompt

4. Treat the package board as the model handoff.
Combine the minimum visual and textual controls needed for consistent generation. Keep it focused on control, not decoration.

5. Encode continuity rules explicitly.
Repeat fragile constraints in both the planning materials and the final prompt:
- fixed character appearance
- fixed spatial layout
- fixed screen direction
- fixed object positions
- fixed action logic

6. Adapt the method to the video type.
Do not overfit to the included sitcom example. Apply the same workflow to action clips, product videos, UGC, ads, tutorials, or short narrative pieces by changing the story logic and asset details, not the underlying process.

## Output Standard

Produce or request a compact preproduction package with these sections:
- creative brief
- Plan Demo
- character definitions
- scene layout definition
- camera blocking definition
- storyboard beats
- package board notes
- continuity constraints
- final generation prompt
- optional release copy

When the user wants only part of the pipeline, still preserve the dependency order. For example, if they ask for a storyboard, infer or request enough character, scene, and camera information to keep the storyboard usable.

## Adaptation Rules

- For dialogue scenes, prioritize screen direction, reverse-shot logic, and room continuity.
- For action scenes, prioritize chase axis, stunt readability, spatial geography, and cause-effect clarity.
- For product or UGC videos, prioritize selling point order, hero object visibility, hand interactions, and environment consistency.
- For short comedy or twist endings, prioritize hook timing, reveal framing, and reaction coverage.

## Resource Use

Read [references/workflow-blueprint.md](references/workflow-blueprint.md) for the canonical step order and deliverable shape.

Read [references/adaptation-guide.md](references/adaptation-guide.md) when the request involves a specific video category or the user wants to adapt the workflow beyond the included examples.

Read [references/example-map.md](references/example-map.md) when you need to locate bundled example materials inside this repository.

Use the existing repository assets and examples as reference material, but do not copy their genre assumptions unless the user asks for that exact style.
