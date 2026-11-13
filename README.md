# Game AI Brainstorming Template

A project template for exploring game ideas with AI. Start with a one-line spark, branch freely, and deepen the ideas that interest you.

## Phases and outputs

Our workflow adapts the [Design Council’s Double Diamond](https://www.designcouncil.org.uk/our-resources/the-double-diamond/) for exploratory game brainstorming. The output names and definitions below are our own.

| Phase | Output | Question | Depth |
|---|---|---|---|
| **Discover** | **Spark** | What caught our imagination? | A one-liner that kicks off an idea. It may be abstract, ambiguous, or impossible to picture yet. No playable explanation is required. |
| **Define** | **Concept** | How could this become something you play? | A playable definition: what you do, what happens, and how gameplay works, supported by visual pitches. |
| **Develop** | **Direction** | How does it fit together and sustain interest? | A holistic view of mechanics, theme, player experience, depth, and potential to grow. Include images and references that establish art style, atmosphere, and how the game fits together. |
| **Deliver** | **Blueprint** | What references inform each part of this game, and how will we adapt them? | An analyzed reference matrix covering every relevant design area, connecting specific references to intended design choices, adaptations, and unresolved questions. |

**Spark → Concept → Direction → Blueprint** describes increasing depth, not a mandatory march toward one winner. Every phase has its own deliverable.

Ideas can branch from branches, combine, or depart from their original starting point. Each branch can move at its own pace. Define captures a temporary focus; it does not bind the exploration to an original problem. Discover is complete with a one-liner, even when we cannot yet imagine how it plays.

## Blueprint reference matrix

Develop establishes the overall direction, including visual references for art style and atmosphere. Deliver turns that direction into a reference matrix: a concrete analysis of what informs each part of the game and how those influences work together.

Cover every relevant area: core gameplay, controls, movement, camera, challenge and balancing, level or encounter design, progression, economy, metagame when applicable, UI and feedback, art, animation, and audio. Add areas the concept needs; mark irrelevant areas as not applicable rather than inventing systems to fill the matrix.

| Design area | Reference and evidence | Specific element | Adaptation for this game | Fit and open questions |
|---|---|---|---|---|
| Camera, controls, balancing, etc. | Named game or other source, with a link, image, or video timestamp where useful | The precise behavior, quality, or relationship we are studying | What we take, change, or combine, and why | How it supports the direction, conflicts with other choices, and what still needs testing |

Analyze specific elements rather than listing game names or assembling a mood board. A reference for camera behavior does not imply borrowing its controls or art style. Several references can inform one area, and one reference can inform several areas for different reasons. Distinguish observed behavior from interpretation and proposed design choices; do not invent hidden balancing formulas or unsupported details.

References support original ideas rather than requiring every idea to match an existing game. If no useful reference is known, identify the original proposal and the uncertainty to investigate. Finish with a synthesis of how the choices fit together, especially dependencies such as camera and controls or progression and balancing. A prototype can test the remaining questions, but the Blueprint’s central deliverable is the reference matrix and its analysis.

## Discover sparks

Read [tai-brainstorm-discover](skills/tai-brainstorm-discover/SKILL.md), or ask your AI tool to use it:

- “Use tai-brainstorm-discover with this spark: a city that dreams.”
- “Branch these sparks: gardening with gravity; a dungeon that wants you to leave.”
- “Discover more sparks by casualizing this combat mechanic.”

Supply one or several starting sparks. If none are available, the skill asks for them. It generates new one-liners using varied techniques, including genre mixing, hardcorizing casual mechanics, casualizing hardcore mechanics, SCAMPER transformations, and unexpected associations. Sparks remain sparks; gameplay definitions belong to Define.

Only the Discover skill is implemented so far. The other phases describe the intended workflow.

## HTML idea map

The offline [HTML map](assets/map.html) stays available as a shared asset for visualizing branches and combinations. It supports parent relationships, search, status filters, and idea details without a server or external libraries. See [the map data format](assets/map-format.md) when populating it.

The map is optional during Discover; generating sparks does not require creating folders or individual files. Clicking a map card changes the view, not an idea’s maturity or the user’s decisions.

## Working with this template

Create a repository using GitHub’s **Use this template**, clone it, and open it in your AI tool. Ask the agent to read [AGENTS.md](AGENTS.md) if it does not do so automatically. Skills are project-local Markdown instructions; no plugin installation is needed.

All skills use the **TAI — Tairos Artificial Intelligence** prefix: `tai-<skill-name>`. Keep the skill folder and its frontmatter name identical. Edit instructions and assets directly; template copies do not automatically receive future updates.

## License

[MIT](LICENSE).
