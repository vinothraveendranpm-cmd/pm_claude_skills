---
name: rapid-prototype
description: Instantly spin up clickable web app prototypes, internal tools, and proof-of-concepts from rough ideas — no engineering needed. Use this skill whenever someone wants to prototype, mock up, or quickly build a web app, internal tool, landing page, form, dashboard, or any scrappy UI. Trigger on phrases like "can you build", "mock this up", "spin up", "prototype", "I need a quick tool", "proof of concept", "POC", "rough version", or "I don't want to wait for engineering". Works with vague ideas (1 sentence) all the way to detailed specs.
---

# Rapid Prototype Skill

Turn ideas — no matter how rough — into real, clickable web prototypes fast. No waiting on engineering. No wireframing tools. Just describe what you need and get a working prototype with realistic fake data.

---

## Step 1: Clarify the Idea (Quickly!)

If the user gives a vague idea, ask **only the most essential questions** — max 2-3, in one go. Don't over-interview. The goal is to unblock, not to spec.

Key things to extract:
- **Who uses this?** (internal team, customers, a specific role like "sales ops")
- **Core action:** What's the ONE thing someone does in this tool? (view data, submit a form, track progress, compare options)
- **Any data or fields to show?** (if not provided, invent realistic fake data yourself)

If the idea has enough to start, **just build it** — don't ask. You can always iterate.

---

## Step 2: Design Thinking Before Building

Before writing a single line of code, commit to a clear design direction:

- **Purpose**: What problem does this solve? Who's the user?
- **Tone**: Pick a bold aesthetic that fits the tool's context:
  - Internal ops tool → clean, utilitarian, data-dense
  - Customer-facing → polished, trustworthy, branded
  - Scrappy POC → fast, functional, minimal chrome
- **The one memorable thing**: What will make this prototype feel *real* and not like a template?

Avoid generic AI aesthetics — no purple gradients, no Inter font, no cookie-cutter layouts.

---

## Step 3: Build the Prototype

Always output a **single self-contained React (.jsx) artifact** — no separate files, no external dependencies beyond what's available.

### What to always include:

**✅ Realistic Fake Data**
- Never use "Lorem ipsum" or placeholder text like "User 1", "Item A"
- Invent believable names, numbers, statuses, and dates
- Make the data tell a story (e.g., a sales pipeline with deals in different stages)

**✅ Clickable Interactions**
- Buttons should DO something — filter, open a modal, change state, submit
- Navigation tabs/sidebar should switch views
- Forms should show a success state when submitted
- Use `useState` to manage all interactions

**✅ Production-Grade Visual Design**
- Use Tailwind utility classes for layout and spacing
- Choose distinctive typography (import from Google Fonts via @import in a style tag if needed)
- Use a strong color palette with CSS variables
- Add micro-animations for state changes (hover, active, transitions)
- Avoid solid white/grey backgrounds — add depth with subtle gradients or textures

**✅ At Least 2 States**
Every good prototype shows more than one screen or state:
- Empty state + populated state
- List view + detail/modal view
- Form + success confirmation
- Default + filtered/searched result

### Available libraries (use freely):
- `lucide-react` for icons: `import { Search, Plus, Filter } from "lucide-react"`
- `recharts` for charts: `import { BarChart, LineChart } from "recharts"`
- `shadcn/ui` for components: `import { Badge, Button } from "@/components/ui/..."`
- Tailwind CSS for all styling

### What NOT to do:
- ❌ Don't use `localStorage` or `sessionStorage` (not supported)
- ❌ Don't create separate CSS or JS files
- ❌ Don't use placeholder copy — invent real-feeling content
- ❌ Don't make it look like a wireframe — make it look like a real product

---

## Step 4: After Building — Offer Next Steps

End every prototype with a short, friendly prompt like:

> "Here's your prototype! Want me to add [specific feature], swap out the data, or make it look more like your brand?"

Suggest 2-3 concrete next iterations based on what you built:
- Add a real form submission flow
- Connect it to an API
- Export as a shareable HTML file
- Add user authentication UI
- Add a mobile-responsive layout

---

## Handling Different Input Types

### 🟡 Vague idea ("I need something to track team requests")
→ Make reasonable assumptions, invent a realistic use case, build immediately, explain your assumptions at the end.

### 🟠 Feature list ("I need a form with name, email, department, and a priority dropdown")
→ Build it with styled components, fake submission handling, and a confirmation state. Add any obvious missing UX (validation, error states).

### 🔵 Detailed spec or screenshot description
→ Follow it closely. Fill in any gaps with good judgment. Match the described layout and flow.

---

## Prototype Quality Checklist

Before outputting, verify:
- [ ] Fake data is realistic and specific (not generic)
- [ ] At least one interactive element works (click, filter, submit)
- [ ] Design has a clear aesthetic POV — not generic
- [ ] At least 2 UI states are visible or reachable
- [ ] No Lorem Ipsum anywhere
- [ ] Single self-contained .jsx file
