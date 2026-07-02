---
name: "Himanshu Shekhar GitHub Profile"
description: "A GitHub-native README that preserves the hshekhar.bhayanak.net terminal shell identity."
colors:
  storm-shell: "#24283b"
  storm-ink: "#c0caf5"
  prompt-violet: "#bb9af7"
  path-blue: "#7aa2f7"
  dollar-green: "#9ece6a"
  ghost-output: "#a9b1d6"
  badge-ink: "#1a1b26"
typography:
  display:
    fontFamily: "JetBrains Mono, monospace"
    fontSize: "GitHub default heading scale"
    fontWeight: 500
    lineHeight: "normal"
    letterSpacing: "normal"
  body:
    fontFamily: "GitHub default / JetBrains Mono where explicitly rendered"
    fontSize: "GitHub default body scale"
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: "normal"
  label:
    fontFamily: "JetBrains Mono, monospace"
    fontSize: "inherit"
    fontWeight: 500
    lineHeight: "normal"
    letterSpacing: "normal"
components:
  prompt-line:
    backgroundColor: "{colors.storm-shell}"
    textColor: "{colors.storm-ink}"
    typography: "{typography.label}"
  command-label:
    backgroundColor: "{colors.prompt-violet}"
    textColor: "{colors.badge-ink}"
    typography: "{typography.label}"
  text-link:
    backgroundColor: "{colors.storm-shell}"
    textColor: "{colors.path-blue}"
    typography: "{typography.body}"
---

# Design System: Himanshu Shekhar GitHub Profile

## 1. Overview

**Creative North Star: "The Mischief Terminal, rendered as Markdown"**

The README should feel like the public GitHub companion to `hshekhar.bhayanak.net`, not a separate profile template. Preserve the terminal-native rhythm: command lines, output blocks, short signals, arrow links, and a compact public-project inventory. The GitHub surface cannot carry the full Astro/Tailwind shell, so the design translates the site identity into Markdown structure instead of fake terminal decoration.

The personal site is the canonical brand source: Tokyo Night Storm, JetBrains Mono, prompt/output sequencing, flat surfaces, no cards, no gradients, no resume sterility. The README must stay readable inside GitHub's renderer, so terminal flavor should clarify sections rather than force inaccessible color tricks GitHub Markdown cannot control.

**Key Characteristics:**

- GitHub-native Markdown with terminal prompt cadence.
- Public-project focus: `CardsAgainstBhayanak`, `BhayanakCast`, `BhayanakBot`, `AntSimulation`, and `hshekhar.bhayanak.net`.
- Tokyo Night identity carried through names, ordering, code labels, and prompt copy.
- Flat, text-first hierarchy. No badge wall, no card grid, no decorative widgets as primary proof.
- Contact path visible at the top and bottom.

## 2. Colors

The palette is inherited from `hshekhar.bhayanak.net`: Tokyo Night Storm with violet prompt identity, blue links/paths, green prompt punctuation, and pale lavender ink.

### Primary

- **Prompt Violet** (`prompt-violet`): the identity accent from the personal site. In README work, reference it through naming and badge choices rather than forcing unsupported inline color.
- **Path Blue** (`path-blue`): navigational/link role. GitHub controls link color in rendered Markdown; keep link copy path-like and explicit.
- **Dollar Green** (`dollar-green`): prompt punctuation role. Use `$` and shell-command language sparingly to preserve the site voice.

### Neutral

- **Storm Shell** (`storm-shell`): canonical personal-site background, not directly applied to GitHub README body.
- **Storm Ink** (`storm-ink`): canonical readable terminal text.
- **Ghost Output** (`ghost-output`): secondary terminal output; never use weak muted text as essential copy in GitHub images or badges.
- **Badge Ink** (`badge-ink`): text color on violet command labels in the site.

### Named Rules

**The Brand Source Rule.** If GitHub README styling and the personal site diverge, the personal site decides the brand language; GitHub decides the rendering constraints.

**The Role Color Rule.** Violet is prompt identity, blue is path/link, green is prompt punctuation or success. Do not turn the README into generic purple tech branding.

## 3. Typography

**Display Font:** GitHub heading renderer; personal-site equivalent is JetBrains Mono  
**Body Font:** GitHub body renderer; personal-site equivalent is JetBrains Mono  
**Label/Mono Font:** Markdown code spans as the GitHub-safe mono layer

**Character:** The site is mono-forward, but GitHub README typography is partly controlled by GitHub. Preserve the terminal feel through command syntax, code spans, compact labels, and short output blocks. Do not fight the renderer with HTML-heavy typography.

### Hierarchy

- **Display** (GitHub `h1`): one identity line only.
- **Headline** (GitHub `h2`): command-like section names such as `cat signal.md`, `ls proof-points`, and `cat contact.md`.
- **Title** (GitHub `h3`): project names and focused proof labels.
- **Body** (GitHub paragraph/list): concise output copy, ideally below 75ch where practical.
- **Label** (Markdown code spans): stack tags, command fragments, repo names, and terminal-flavored metadata.

### Named Rules

**The Markdown Terminal Rule.** Use prompts and filenames as information architecture, not decoration. `cat signal.md` is useful because it tells the reader what follows.

**The One Mono Layer Rule.** Use code spans for stack labels and commands. Do not wrap whole paragraphs in code blocks; that hurts scanning and accessibility.

## 4. Elevation

This system is flat. The personal site uses no cards or shadows; the README should also avoid card-like HTML tables, nested panels, and soft visual containers. Depth comes from command sequencing, horizontal rules, headings, and concise output.

### Named Rules

**The Flat Shell Rule.** Do not add cards to make the README feel designed. Make the content sharper instead.

**The No Widget-as-Proof Rule.** Stats, streaks, and snakes are secondary activity signals. They cannot replace project proof.

## 5. Components

### Prompt Section

Use a heading that reads like a shell command, followed by Markdown output. Example: `## $ cat signal.md`.

- **Shape:** text heading + output list.
- **Role:** maps personal-site prompt rhythm to GitHub.
- **Constraint:** do not overuse if it makes the README noisy.

### Proof Point

Each focused public project gets a `###` heading, one compact proof paragraph, and a single stack line.

- **Shape:** project link, proof-oriented summary, code-span stack tags.
- **Order:** lead with the user-selected focus set.
- **Constraint:** no private-project references.

### Contact Links

Arrow-prefixed links echo the personal site.

- **Shape:** `→ label`.
- **Placement:** top row and final contact section.
- **Constraint:** contact remains visible without animation or images.

## 6. Do's and Don'ts

### Do:

- **Do** preserve the terminal rhythm from `hshekhar.bhayanak.net`: prompt, command, output, link.
- **Do** focus the public project set: `CardsAgainstBhayanak`, `BhayanakCast`, `BhayanakBot`, `AntSimulation`, and `hshekhar.bhayanak.net`.
- **Do** use code spans for stack labels and repo names.
- **Do** keep GitHub stats below the proof sections.
- **Do** keep contact links visible near the top and bottom.

### Don't:

- **Don't** highlight private projects or internal work.
- **Don't** create a generic badge-wall profile where shields and stats carry the whole identity.
- **Don't** make it feel like a corporate resume page: dry, buzzword-heavy, and interchangeable.
- **Don't** create unreadable terminal cosplay: giant code blocks, low contrast images, hidden links, or gimmicks that block scanning.
- **Don't** use purple gradients, neon hacker glow, glassmorphism, decorative side-stripe borders, rounded cards, or soft shadows.
