# Visual Guidance

Reference for recommending specific, actionable visuals in presentation outlines. Load this when the outline needs detailed visual recommendations — especially for technical, data-heavy, or educational presentations.

---

## Visual Selection Matrix

Choose visuals based on what the slide communicates:

| Communication goal | Recommended visual | Avoid |
|---|---|---|
| Comparison of quantities | Horizontal or vertical bar chart | Pie chart with >5 segments |
| Trend over time | Line chart or area chart | Bar chart (harder to see trends) |
| Part of a whole | Pie chart (≤5 segments), stacked bar, treemap | Tables of percentages |
| Process or workflow | Flowchart, swim lane diagram | Bullet list of steps |
| Hierarchy or structure | Org chart, tree diagram | Nested bullet points |
| Relationship between entities | Network diagram, Venn diagram | Paragraph descriptions |
| Geographic distribution | Map with data overlay | Table of locations |
| Timeline or sequence | Timeline graphic, Gantt chart | Bullet list with dates |
| Before/After | Side-by-side comparison, split slide | Sequential slides |
| Architecture or system design | Component diagram, C4 model | Wall of text description |
| Data table (few rows) | Clean table with highlight row | Chart (overkill for small data) |
| Single key metric | Large number with context label | Buried in a paragraph |

---

## Chart Best Practices

### Bar Charts
- Use horizontal bars when labels are long (category names)
- Use vertical bars for time-series with few data points
- Always start the y-axis at zero — truncated axes mislead
- Highlight the bar that matters with a contrasting color

### Line Charts
- Use for 3+ time periods — fewer points work better as bars
- Limit to 4 lines maximum — beyond that, split into multiple charts
- Label lines directly rather than using a legend (reduces eye movement)
- Use consistent time intervals on the x-axis

### Pie Charts
- Maximum 5 segments — more than that, use a bar chart
- Order segments by size (largest to smallest, clockwise from 12 o'clock)
- Pull out the segment you want to emphasize
- Never use 3D pie charts — they distort proportions

### Tables
- Use for exact values when precision matters
- Maximum 5 columns, 7 rows per slide
- Highlight the key row or column with shading
- Align numbers to the right, text to the left

---

## Diagram Types

### Flowcharts
- Use for processes with decision points
- Flow left-to-right or top-to-bottom (never both)
- Limit to 8–10 nodes per diagram — split complex flows across slides
- Use consistent shapes: rectangles for steps, diamonds for decisions, ovals for start/end

### Architecture Diagrams
- Show components as boxes with clear labels
- Use arrows for data/request flow — label the arrows
- Group related components with dotted boundaries
- Include external systems at the edges
- Color-code by layer (frontend, backend, data, external)

### Timeline Graphics
- Use for project phases, product roadmaps, historical sequences
- Place the current moment clearly (if relevant)
- Group into 3–5 phases maximum
- Include key milestones as callouts, not every detail

### Matrices and Frameworks
- 2x2 matrices: Use for positioning, prioritization (impact vs effort, etc.)
- Label all four quadrants with clear category names
- Place items as dots/icons within quadrants
- The quadrant names should tell the story ("Quick Wins", "Big Bets", etc.)

---

## Visual Design Principles

### Cognitive Load Reduction
- **One visual per slide** — competing visuals split attention
- **Remove chartjunk** — no 3D effects, no gradient fills, no decorative gridlines
- **Use whitespace** — crowded slides feel overwhelming and reduce comprehension
- **Consistent color palette** — 3–5 colors maximum across the entire deck
- **Progressive reveal** — in live presentations, build complex diagrams step by step

### Visual Hierarchy
- **Size signals importance** — the most important element should be largest
- **Color signals attention** — use accent color sparingly for emphasis
- **Position signals priority** — top-left gets read first (in LTR cultures)
- **Contrast signals grouping** — similar elements look similar, different elements look different

### Data Visualization Principles (Tufte-inspired)
- **Maximize data-ink ratio** — every pixel should convey information
- **Avoid chart decorations** — no clip art, no background images behind charts
- **Show context** — include comparison points (previous period, benchmark, target)
- **Label directly** — put labels on data points, not in legends
- **Use small multiples** — repeat the same chart for different categories rather than cramming everything into one

---

## Icon Recommendations

When suggesting icons in outlines, be specific about what to depict:

| Concept | Icon suggestion |
|---|---|
| Growth/increase | Upward trending arrow or graph line |
| Security/protection | Shield icon |
| Speed/performance | Speedometer or lightning bolt |
| Collaboration | Connected people or handshake |
| Integration | Puzzle pieces or interlocking gears |
| Cost/money | Dollar sign or coins stack |
| Time/efficiency | Clock or hourglass |
| Global/international | Globe icon |
| Data/analytics | Bar chart or dashboard icon |
| Innovation | Lightbulb icon |
| Warning/risk | Triangle alert icon |
| Success/completion | Checkmark or trophy |

---

## Layout Patterns

Common slide layouts for AI tool compatibility:

| Layout name | Description | Best for |
|---|---|---|
| **Title + subtitle** | Large title, supporting subtitle | Section openers, title slides |
| **Big number** | One metric, large, with context | KPI highlights, impact stats |
| **Two-column** | Content split left/right | Comparisons, before/after |
| **Three-column** | Three equal sections | Feature highlights, pillars |
| **Image + text** | Half image, half content | Story slides, product shots |
| **Full image** | Image with minimal text overlay | Keynote mood slides |
| **Diagram** | Central visual with labels | Architecture, process flow |
| **Timeline** | Horizontal timeline with milestones | Roadmaps, project phases |
| **Grid** | 2x2 or 3x3 content blocks | Feature grids, team slides |
| **Quote** | Large quote with attribution | Customer testimonials, vision |

---

## AI Tool Visual Descriptions

When writing visual recommendations for AI presentation tools, use this format:

**Effective (specific, parseable):**
- "Horizontal bar chart comparing current vs. target for 5 KPIs"
- "3-phase timeline showing Discovery → Development → Launch with dates"
- "Architecture diagram: User → API Gateway → Microservices → Database"
- "2x2 matrix with axes: Impact (low/high) and Effort (low/high)"

**Ineffective (vague, unparseable):**
- "Add a chart"
- "Include a visual"
- "Something to show the data"
- "An engaging graphic"
