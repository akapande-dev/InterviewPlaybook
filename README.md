# 📖 InterviewPlaybook

A clean, fully static HTML page that consolidates the most essential technical interview preparation resources in one place — DSA, JavaScript, React, System Design, and Claude Code.

---

## 🌐 Live Preview

Website: https://akapande-dev.github.io/InterviewPlaybook/

---

## 📁 Project Structure

```
InterviewPlaybook/
├── InterviewPlaybook.html      # Main website (single file)
├── PDFs/
│   └── javascript-questions.pdf   # 100 JS Interview Questions (add your own copy)
└── README.md
```

---

## 📚 What's Inside

| Section | Resource | Questions / Content |
|---|---|---|
| 🧩 DSA Practice | [Striver's 79 Last Moment Sheet](https://takeuforward.org/dsa/strivers-79-last-moment-dsa-sheet-ace-interviews) | 79 curated problems |
| ⚡ JavaScript | Local PDF (`PDFs/javascript-questions.pdf`) | 100 questions |
| ⚛️ React | [GreatFrontEnd — 100 React Questions](https://www.greatfrontend.com/blog/100-react-interview-questions-straight-from-ex-interviewers) | 100 questions |
| 🏗️ System Design | [GeeksforGeeks Complete Roadmap](https://www.geeksforgeeks.org/system-design/complete-roadmap-to-learn-system-design/) | Full roadmap |
| 🤖 Claude Code | [SFEIR Institute Interview Guide](https://institute.sfeir.com/en/claude-code/claude-code-resources/interview/) | 27 Q&As (Junior / Mid / Senior) |

---

## 🤖 Claude Code Section — Details

The Claude Code card is the centrepiece of the page. It covers:

**File Structure Reference**
```
Project/
├── CLAUDE.md                  # Team conventions (versioned)
├── .claude/
│   ├── settings.json          # Shared permissions
│   └── CLAUDE.md              # Repo-level instructions
└── src/
    └── CLAUDE.md              # Folder-specific instructions
```

**27 Interview Questions across 3 levels:**

- **Junior (9 Qs · 20–30 min)** — Installation, CLI basics, slash commands (`/help`, `/clear`, `/compact`), plan vs implementation mode
- **Mid-Level (9 Qs · 30–40 min)** — CLAUDE.md memory system, permissions via `.claude/settings.json`, Git integration, headless mode (`-p` flag), token optimization, hooks
- **Senior (9 Qs · 40–50 min)** — CI/CD integration, MCP (Model Context Protocol), multi-developer memory architecture, subagents, monorepo handling, enterprise security

---

## ✏️ Personalisation

Before deploying, update these three things in `InterviewPlaybook.html`:

**1. Your photo**
Find the `<img>` tag inside `.creator-avatar` and replace the `src` with your actual photo path:
```html
<!-- Before -->
<img src="https://placehold.co/100x100/..." alt="Creator photo" />

<!-- After -->
<img src="images/your-photo.jpg" alt="Your Name" />
```

**2. Your name**
Search for `Your Name` (appears 3 times) and replace with your real name.

**3. Your LinkedIn URL**
Find the LinkedIn anchor tag and update the `href`:
```html
<a class="linkedin-btn" href="https://linkedin.com/in/your-actual-profile" ...>
```

**4. JavaScript PDF**
Place your PDF file at `PDFs/javascript-questions.pdf` relative to the HTML file. The link is already wired up.

---

## 🎨 Design System

| Token | Value | Used for |
|---|---|---|
| Background | `#0a0e1a` | Page background |
| Surface | `#111827` | Card backgrounds |
| Accent Blue | `#4f8ef7` | Nav logo, React card, default glow |
| Accent Green | `#34d399` | DSA card, creator badge, live dot |
| Accent Orange | `#fb923c` | JavaScript card |
| Accent Purple | `#a78bfa` | System Design card, gradient |
| Accent Pink | `#f472b6` | Claude Code card |

**Fonts (loaded from Google Fonts):**
- `Space Grotesk` — headings and display text
- `Inter` — body copy
- `JetBrains Mono` — tags, code snippets, file structure

---

## 🚀 Deployment

This is a single static HTML file. You can host it anywhere:

**GitHub Pages**
1. Push the project to a GitHub repo
2. Go to Settings → Pages → select `main` branch
3. Your site is live at `https://<username>.github.io/<repo>/InterviewPlaybook.html`

**Netlify / Vercel**
Drop the project folder into the Netlify or Vercel dashboard for instant deployment.

**Local**
Simply double-click `InterviewPlaybook.html` or serve with:
```bash
npx serve .
# or
python -m http.server 8080
```

> **Note:** The PDF link (`PDFs/javascript-questions.pdf`) requires a server or local file access. It will not work if the HTML is opened as a raw `file://` URL in some browsers due to security restrictions. Use `npx serve` or any local server for full functionality.

---

## 📱 Responsive Behaviour

| Breakpoint | Layout |
|---|---|
| `> 640px` | 2-column card grid, visible nav links |
| `≤ 640px` | Single-column stack, nav links hidden |

The Claude Code wide card always spans full width on all screen sizes.

---

## 🛠️ Tech Stack

- Plain HTML5 + CSS3 (no frameworks, no JavaScript)
- Google Fonts (Space Grotesk, Inter, JetBrains Mono)
- CSS custom properties for theming
- CSS Grid for responsive layout
- `backdrop-filter` for frosted-glass nav

No dependencies. No build step. No npm. Just open and use.

---

## 📄 License

Personal use. All linked external resources belong to their respective owners (TakeUForward, GreatFrontEnd, GeeksforGeeks, SFEIR Institute, Anthropic).
