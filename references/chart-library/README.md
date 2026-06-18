# McKinsey Chart Library

A pattern catalog distilled from McKinsey's "Week in Charts" column. Plugged into `/ai-presentation-builder` so the skill can generate **original, editable** python-pptx charts in McKinsey's visual style.

## What's in here

```
chart-library/
├── README.md             ← this file
├── SOURCES.md            ← citation + copyright note
├── SKILL_INTEGRATION.md  ← snippet to merge into ai-presentation-builder/SKILL.md
└── patterns/             ← reusable chart pattern specs
    ├── 01-horizontal-bar-with-delta.md
    ├── 02-dual-panel-bar.md
    ├── 03-stacked-bar.md
    ├── 04-line-with-annotations.md
    ├── 05-combined-bar-and-line.md
    └── 06-small-multiples.md
```

## How the skill uses this

When `/ai-presentation-builder` needs to generate a chart, it reads `patterns/00-shared-design-rules.md`, matches the data shape to one of the `patterns/*.md` specs, and uses that pattern's python-pptx recipe, headline conventions, color rules, and source-line format.

The chart is built **from scratch** using python-pptx. McKinsey's chart images are NOT embedded — they are reference only.

## Coverage

Six reusable chart patterns covering the most common consulting chart types, distilled from the visual conventions of McKinsey's "Week in Charts" column. Each pattern is an original spec — anatomy, design rules, python-pptx recipe — not a copy of any source chart.

## Copyright

All chart content © McKinsey & Company. This library is for personal pattern study. Charts produced by your skill must be original work using your own data — they should be McKinsey-*styled*, never McKinsey-*copied*.

See `SOURCES.md` for the full citation list.
