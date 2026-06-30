# AI OS — Design System

> A premium GitHub profile design system inspired by Apple, Linear, Vercel, and modern AI interfaces.

---

## Design Philosophy

| Principle | Description |
|-----------|-------------|
| Minimal | Nothing unnecessary. Every element serves a purpose. |
| Luxury | Premium materials, refined spacing, intentional hierarchy. |
| Glassmorphism | Subtle glass surfaces with backdrop blur and light borders. |
| Monochrome | Black base with carefully desaturated accent colors. |
| AI Dashboard | Feels like a futuristic operating system control center. |
| Elegant | Refined typography, perfect rhythm, calm presence. |

**Keywords:** Minimal · Luxury · Premium · Glassmorphism · Black · Apple · AI Dashboard · Futuristic · Elegant · Sophisticated · Whitespace

---

## Color System

### Base Colors

| Token | Hex | Usage |
|-------|-----|-------|
| `--bg-primary` | `#050505` | Main background |
| `--bg-secondary` | `#0B0B0B` | Card/section backgrounds |
| `--bg-tertiary` | `#111111` | Elevated surfaces |
| `--glass` | `rgba(255,255,255,0.04)` | Glass surface |
| `--glass-medium` | `rgba(255,255,255,0.06)` | Glass surface (hover) |
| `--glass-heavy` | `rgba(255,255,255,0.10)` | Glass surface (active) |
| `--glass-border` | `rgba(255,255,255,0.08)` | Glass border |
| `--glass-border-hover` | `rgba(255,255,255,0.14)` | Glass border (hover) |

### Text Colors

| Token | Hex | Usage |
|-------|-----|-------|
| `--text-primary` | `#FFFFFF` | Headings, primary content |
| `--text-secondary` | `#A1A1AA` | Body text, subtitles |
| `--text-tertiary` | `#71717A` | Captions, metadata |
| `--text-muted` | `#52525B` | Placeholder, disabled |

### Accent Colors

| Token | Hex | Usage |
|-------|-----|-------|
| `--accent-blue` | `#4CC9F0` | Links, highlights |
| `--accent-cyan` | `#22D3EE` | Secondary accent |
| `--accent-purple` | `#8B5CF6` | Tertiary accent |
| `--accent-green` | `#34D399` | Success, active states |
| `--accent-amber` | `#FBBF24` | Warning, attention |

### Glow Effects

| Token | Value |
|-------|-------|
| `--glow-blue` | `0 0 40px rgba(76,201,240,0.15)` |
| `--glow-purple` | `0 0 40px rgba(139,92,246,0.12)` |
| `--glow-cyan` | `0 0 40px rgba(34,211,238,0.10)` |

> Glows must always be extremely subtle. Never use saturated colors.

---

## Typography

### Font Stack

```
Primary:    Inter
UI:         SF Pro Display / -apple-system
Accent:     Space Grotesk
Monospace:  JetBrains Mono
```

### Scale

| Level | Size | Weight | Line Height | Tracking |
|-------|------|--------|-------------|----------|
| Hero | 56px | 300 (Light) | 1.1 | -0.03em |
| H1 | 40px | 300 (Light) | 1.15 | -0.025em |
| H2 | 32px | 300 (Light) | 1.2 | -0.02em |
| H3 | 24px | 400 (Regular) | 1.25 | -0.015em |
| H4 | 20px | 400 (Regular) | 1.3 | -0.01em |
| Body | 16px | 400 (Regular) | 1.6 | 0em |
| Body Small | 14px | 400 (Regular) | 1.5 | 0em |
| Caption | 12px | 500 (Medium) | 1.4 | 0.02em |
| Overline | 11px | 600 (Semibold) | 1.2 | 0.08em |
| Metric | 28px | 300 (Light) | 1 | -0.02em |

### Rules

- Huge whitespace between sections (64px–96px)
- Large headings with light font weights
- Excellent hierarchy through size and weight, not color
- Nothing should feel crowded

---

## Spacing System

Based on an 8px grid.

| Token | Value |
|-------|-------|
| `--space-1` | 4px |
| `--space-2` | 8px |
| `--space-3` | 12px |
| `--space-4` | 16px |
| `--space-5` | 20px |
| `--space-6` | 24px |
| `--space-8` | 32px |
| `--space-10` | 40px |
| `--space-12` | 48px |
| `--space-16` | 64px |
| `--space-20` | 80px |
| `--space-24` | 96px |

### Layout Rules

- Section spacing: `--space-16` (64px)
- Card padding: `--space-6` (24px)
- Grid gap: `--space-4` (16px)
- Between headings and content: `--space-4` (16px)
- Between form elements: `--space-5` (20px)

---

## Border Radius

| Token | Value | Usage |
|-------|-------|-------|
| `--radius-sm` | 6px | Small elements, badges |
| `--radius-md` | 10px | Buttons, inputs |
| `--radius-lg` | 16px | Cards, panels |
| `--radius-xl` | 24px | Hero section, modals |
| `--radius-full` | 9999px | Avatars, pills |

---

## Glass Components

### Glass Card
```
background: rgba(255,255,255,0.04);
backdrop-filter: blur(20px);
border: 1px solid rgba(255,255,255,0.08);
border-radius: 16px;
```

### Glass Card (Hover)
```
background: rgba(255,255,255,0.06);
border-color: rgba(255,255,255,0.14);
```

### Glass Panel (Hero)
```
background: linear-gradient(
  135deg,
  rgba(255,255,255,0.06) 0%,
  rgba(255,255,255,0.02) 100%
);
backdrop-filter: blur(40px);
border: 1px solid rgba(255,255,255,0.10);
border-radius: 24px;
```

---

## Shadows

| Token | Value |
|-------|-------|
| `--shadow-sm` | `0 1px 2px rgba(0,0,0,0.3)` |
| `--shadow-md` | `0 4px 12px rgba(0,0,0,0.4)` |
| `--shadow-lg` | `0 8px 32px rgba(0,0,0,0.5)` |
| `--shadow-xl` | `0 16px 48px rgba(0,0,0,0.6)` |
| `--shadow-glass` | `0 4px 24px rgba(0,0,0,0.3), inset 0 1px 0 rgba(255,255,255,0.06)` |

---

## Animation

### Duration
| Token | Value |
|-------|-------|
| Instant | 100ms |
| Fast | 200ms |
| Normal | 300ms |
| Slow | 500ms |
| Float | 3000ms+ |

### Timing Functions
| Token | Value |
|-------|-------|
| `--ease-out` | `cubic-bezier(0.16, 1, 0.3, 1)` |
| `--ease-inout` | `cubic-bezier(0.65, 0, 0.35, 1)` |
| `--spring` | `cubic-bezier(0.34, 1.56, 0.64, 1)` |

### Animations Used

- **Pulse**: Subtle opacity pulse for status indicators (4s cycle)
- **Float**: Gentle levitation for hero elements (6s cycle)
- **Gradient**: Slow gradient drift (10s cycle)
- **Spin**: Loading spinners (1s cycle)
- **Typing**: Cursor blink (1s cycle)
- **Particle**: Slow particle drift (20s+ cycle)

---

## Iconography

- Library: **Lucide** / **Heroicons** style
- Stroke width: 1.5px
- Size: 16px–24px for UI, 32px+ for feature icons
- Color: `--text-secondary` by default, `--text-primary` on hover
- All icons must be monochrome — no colored SVG icons

---

## Bento Grid Layout

### Desktop (12 columns)
```
┌─────────────────────────────────────────────────────┐
│                     HERO (12 cols)                    │
├──────────────┬──────────────┬────────────────────────┤
│   ABOUT      │  AI CORE     │   GITHUB STATS         │
│   (4 cols)   │  STATUS      │   (4 cols)             │
│              │  (4 cols)    │                        │
├──────────────┴──────────────┴────────────────────────┤
│             CONTRIBUTION GRAPH (12 cols)              │
├──────────────┬───────────────────┬───────────────────┤
│   STREAK     │   ACTIVITY        │   TECH STACK      │
│   (4 cols)   │   (4 cols)        │   (4 cols)        │
├──────────────┴───────────────────┴───────────────────┤
│             FEATURED PROJECTS (12 cols)               │
├──────────────┬───────────────────┬───────────────────┤
│  LEARNING    │   CONNECT         │   METRICS         │
│  ROADMAP     │   (4 cols)        │   (4 cols)        │
│  (4 cols)    │                   │                   │
├──────────────┴───────────────────┴───────────────────┤
│                     FOOTER (12 cols)                  │
└─────────────────────────────────────────────────────┘
```

### Tablet (8 columns)
- All sections collapse to 8 or 4 columns
- Cards stack vertically within sections

### Mobile (4 columns)
- Single column layout
- All cards full width
- Reduced padding and font sizes

---

## Component Specifications

### Hero Card
- 12 columns wide
- 2 rows (internal flex layout: text left, illustration right)
- Title: 56px Light, Name
- Subtitle: 20px, secondary text
- Description: 16px, secondary text
- Buttons: Glass style, rounded-lg
- Right side: Abstract illustration (SVG)

### AI Core Status
- 4 columns
- Header: System icon + "AI Core" label
- Progress bars: Label + percentage + thin bar
- Max 6 metrics
- Each bar: 4px height, rounded, accent color fill

### GitHub Stats
- 4 columns
- Integrates `github-readme-stats` API
- Custom styling via CSS parameters
- Compact layout

### Contribution Graph
- 12 columns
- Uses `github-contribution-grid-snake` GIF
- Custom dark theme
- Full width

### Tech Stack
- 4 columns
- Monochrome SVG icons in a grid
- Organized: Languages, Frameworks, Tools, AI/ML
- Each icon: 28px, glass background on hover

### Featured Projects
- 12 columns
- 3 equal cards
- Each: Title, description, tech tags, link button
- Glass card style

---

## GitHub Integration

### API Endpoints Used
```
Stats:        https://github-readme-stats.vercel.app/api
Streak:       https://github-readme-streak-stats.herokuapp.com
Trophy:       https://github-profile-trophy.vercel.app
Snake:        https://github.com/Nikhilrai27/Nikhilrai27/blob/output/github-contribution-grid-snake-dark.svg
```

### Theme Configuration
All widgets must use custom dark theme parameters:
```
?theme=dark&bg_color=050505&border_color=rgba(255,255,255,0.08)
```

---

## Accessibility

- Maintain minimum 4.5:1 contrast ratio for all text
- Font sizes never below 12px
- Semantic HTML structure with proper heading hierarchy
- All images require descriptive alt text
- Interactive elements have visible focus states
- Animation respect `prefers-reduced-motion`

---

## File Structure

```
/
├── .github/
│   └── workflows/
│       ├── snake.yml
│       └── metrics.yml
├── assets/
│   └── svg/
│       ├── hero-neural-network.svg
│       ├── particles-bg.svg
│       ├── neural-lines.svg
│       ├── status-pulse.svg
│       ├── glass-sphere.svg
│       └── icons/
│           ├── python.svg
│           ├── fastapi.svg
│           ├── langchain.svg
│           ├── docker.svg
│           ├── postgresql.svg
│           ├── git.svg
│           ├── linux.svg
│           ├── openai.svg
│           └── gemini.svg
├── docs/
│   └── ... (future documentation)
├── DESIGN_SYSTEM.md
└── README.md
```
