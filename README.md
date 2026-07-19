# Presentation Outline Skill for Claude Code

A Claude Code skill that transforms raw information into structured, narrative-driven presentation outlines. Produces outlines optimized for AI presentation tools (Gamma, Beautiful.ai, Tome) and human use.

Combines consulting-grade structure (McKinsey SCR, Pyramid Principle) with storytelling craft (Duarte Sparkline, TED structure) and modern visual design principles.

## Install

Copy the skill directory into your Claude Code skills folder:

```bash
cp -r presentation-outline-skill/ ~/.claude/skills/presentation-outline/
```

The skill activates automatically when you ask Claude Code to create a presentation outline, build a slide deck, design a pitch deck, or structure any kind of talk.

## What It Does

Generates complete presentation outlines with:

- Slide titles, content, and key takeaways
- Narrative structure appropriate to the presentation type
- Specific visual recommendations (chart types, diagrams, layouts)
- Speaker notes with delivery guidance
- Slide-to-slide transitions that maintain narrative flow

## Supported Presentation Types

| Type | Narrative Approach |
|---|---|
| Business proposal / Sales deck | Persuasion Arc (Situation → Complication → Resolution) |
| Investor / Pitch deck | Pitch Structure (Problem → Solution → Traction → Ask) |
| Technical architecture | Technical Flow (Context → Design → Trade-offs → Implementation) |
| Product review / Project update | Status Arc (Progress → Blockers → Decisions) |
| Educational / Workshop | Learning Arc (Hook → Foundation → Build → Apply) |
| Keynote / Conference talk | Story Arc (What Is → What Could Be → New Bliss) |
| Executive briefing | Pyramid + BLUF (Bottom Line Up Front) |
| Internal strategy | Pyramid Principle (Recommendation first) |
| Research presentation | Scientific method adapted |

## Usage Examples

```
Create a 10-slide investor pitch deck outline for an AI-powered customer analytics platform.
```

```
Build a presentation outline for a technical architecture review — audience is engineering leadership, 30 minutes.
```

```
Outline a keynote talk about the future of remote work for a 2000-person conference. 20 minutes.
```

```
Create a quick outline for a 5-minute team update on our Q3 progress.
```

```
Build a sales deck outline for our CRM product targeting mid-market companies. Optimize for Gamma.
```

## Skill Structure

```
presentation-outline-skill/
├── SKILL.md                           # Core skill — process, principles, constraints
├── reference/                         # Deep-dive guides (loaded on demand)
│   ├── narrative-frameworks.md        # Pyramid Principle, SCR, Duarte, pitch structure
│   ├── deck-types.md                  # Templates for 10+ presentation types
│   └── visual-guidance.md             # Chart selection, diagram types, layout patterns
└── examples/                          # Calibration examples
    └── sample-outlines.md             # Full 10-slide example with annotations
```

**Progressive loading:** The core SKILL.md stays in context. Reference files and examples load on demand based on the presentation type.

## Design Decisions

### Why these frameworks?

- **Pyramid Principle** (Minto): Universal business communication structure — lead with the answer
- **SCR** (McKinsey): Creates urgency through the Situation → Complication → Resolution pattern
- **Duarte Sparkline**: Most effective keynote structure — alternating tension between "what is" and "what could be"
- **Guy Kawasaki 10/20/30**: Practical constraint for pitch decks — 10 slides, 20 minutes, 30pt font

### Why per-slide visual recommendations?

Generic "add a chart" instructions are useless for both humans and AI tools. Specific recommendations ("horizontal bar chart comparing current vs. target for 5 KPIs") give presenters clear direction and AI tools parseable instructions.

### Why separation of slide content and speaker notes?

Slides are visual anchors, not scripts. Mixing them produces slides that are too text-heavy to present and too sparse to read. The skill enforces this separation by treating them as distinct output fields.

## Inputs

The skill works best when given:

- **Topic** — what the presentation is about
- **Audience** — who will see it (executives, engineers, investors, students)
- **Goal** — what the audience should think/feel/do after
- **Time/length** — duration or desired slide count
- **Context** — live, async, internal, external

It will ask for missing critical information (audience and goal) but proceed with sensible defaults for optional inputs.

## Limitations

- Does not generate actual slide designs, images, or finished presentations
- Visual recommendations are descriptive, not rendered
- Cannot access real-time data — outlines use placeholder data points that the user must fill
- Optimized for English-language presentations
- Cultural presentation norms vary — the skill defaults to Western business conventions

## Customization Points

- **Slide count**: Override the automatic recommendation with "make it exactly 8 slides"
- **Detail level**: Say "quick outline" for lean output or "detailed with speaker notes" for comprehensive
- **Tool optimization**: Mention "for Gamma" or "for Beautiful.ai" to optimize formatting
- **Tone**: Specify "formal", "casual", "technical", or "inspirational"
- **Audience**: The more specific the audience description, the better the adaptation

## License

MIT
