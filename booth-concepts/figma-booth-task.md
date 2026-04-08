You have access to the Figma MCP server. Use the `generate_figma_design` tool (or equivalent write tool) to build a Web Summit booth design into this file:

**File URL:** https://www.figma.com/design/Ja1TLBEr4h4lDEjKKMMum3/Social-Media-Templates

Create a new page called "Web Summit Booth" in that file, and build the following design on it.

---

## WHAT TO BUILD: Concept 1 — "The Hub"

A trade show booth spread representing two 3×3m walls side by side. Total frame size: 6000×3000px. Name the frame "Booth Spread — The Hub".

---

## BRAND TOKENS

- Background: #141C22
- Accent gradient: #00C2E0 (teal) → #4ADE5C (electric green), left to right
- Hero text: #E8F5F2
- Secondary text: #7BB5A8
- Font: Outfit (already in the file) — weights 800, 600, 400
- Aurora effect: soft radial glow, #00C2E0 top-right, #4ADE5C bottom-left

---

## LAYOUT

**Wall 1 (left half, 0–3000px):**

Text block, top-left area (x:120, starting y:180):
- "VLS SOLUTIONS" — Outfit 600, 64px, #00C2E0, letter-spacing 4
- Thin separator line below (x:120, w:480, 2px, #00C2E0 30% opacity)
- Eyebrow: "AI MARKETPLACE INFRASTRUCTURE" — Outfit 600, 42px, gradient fill (#00C2E0→#4ADE5C), letter-spacing 4
- Headline line 1: "One engine." — Outfit 800, 260px, fill #E8F5F2, letter-spacing -6
- Headline line 2: "Every market." — Outfit 800, 260px, gradient fill (#00C2E0→#4ADE5C), letter-spacing -6
- Tagline: "The AI infrastructure that powers" — Outfit 400, 70px, #E8F5F2
- Tagline line 2: "any service marketplace." — Outfit 400, 70px, #E8F5F2
- Detail: "Deploy in weeks. Scale to millions. Automate everything." — Outfit 400, 50px, #7BB5A8

**Hub visual (centered at the seam, ~x:3000, y:1450):**

This is the central visual metaphor — VLS Engine as a glowing orb connecting everything.

- Large atmosphere glow: circle r:900, fill #00C2E0, opacity 8%, no stroke (soft blur effect)
- Orbital ring 1: circle r:700, no fill, stroke #00C2E0 1px, opacity 15%, dashed
- Orbital ring 2: circle r:500, no fill, stroke #00C2E0 1.5px, opacity 25%, dashed
- Orbital ring 3: circle r:320, no fill, stroke #4ADE5C 2px, opacity 40%, dashed
- Hub glow: circle r:130, fill #00C2E0, opacity 15%
- Hub core: circle r:80, fill gradient radial white center → #00C2E0 edge
- Center dot: circle r:25, fill #FFFFFF, opacity 95%
- Label below hub: "VLS ENGINE" — Outfit 600, 52px, gradient fill, letter-spacing 4, centered at x:3000

**6 service nodes with connection lines from hub:**

Left wall nodes (each: outer glow circle r:40 fill #00C2E0 opacity 12%, inner circle r:22 fill #00C2E0 opacity 85%, dot r:8 white, label below Outfit 400 36px #7BB5A8 letter-spacing 2):
- (450, 240): "Towing"
- (200, 920): "Home Repair"
- (320, 1580): "Plumbing"
- (550, 2350): "Food Delivery"
- (1400, 2650): "Legal Services"
- (2150, 2180): "Healthcare"

Right wall nodes (same style, alternate some with #4ADE5C instead of #00C2E0):
- (3580, 300): "Real Estate"
- (4450, 520): "Logistics"
- (5500, 820): "E-Commerce"
- (5820, 1500): "Finance"
- (5400, 2380): "Procurement"
- (4020, 2680): "Government"

Connection lines from hub (3000,1450) to each node: stroke #00C2E0, width 1.5px, opacity 28%

**Wall 2 (right half, 3000–6000px):**

QR code section, bottom-right (centered around x:5050, y:2420):
- Container: 680×680px square, rx:16, fill #141C22, stroke gradient #00C2E0→#4ADE5C, stroke-width 3
- Three QR corner finder squares inside (top-left, top-right, bottom-left): outer 120×120 stroke #00C2E0 6px, inner 80×80 fill #00C2E0 opacity 70%
- Small grid of squares in the interior for QR data pattern: fill #7BB5A8, opacity 50%
- Label above QR: "SCAN TO TALK TO OUR AI" — Outfit 600, 52px, gradient fill, letter-spacing 3, centered
- Label below: "vls.ai · Try the demo" — Outfit 400, 42px, #7BB5A8, centered
- Tiny note: "[ PLACEHOLDER — SWAP URL BEFORE PRINT ]" — 28px, #7BB5A8, opacity 30%

**Full-width elements:**
- Subtle wall divider: vertical line at x:3000, full height, stroke #00C2E0 opacity 12%
- Bottom accent bar: full-width rect, x:0 y:2945, w:6000 h:55, gradient fill #00C2E0→#4ADE5C, opacity 55%

**Aurora background:**
- Radial glow top-right: large circle at (5400, 0), r:1800, fill #00C2E0, opacity 18%
- Radial glow bottom-left: large circle at (600, 3000), r:1600, fill #4ADE5C, opacity 20%
- Center glow: circle at (3000, 1500), r:1200, fill #00C2E0, opacity 7%

---

## IMPORTANT NOTES
- Gradient fills on text must be native Figma gradients (not SVG mask tricks) — this is the whole reason we're doing this in Figma
- Group elements logically: background, aurora, hub-visual, nodes, wall1-text, wall2-qr, accent-bar
- Keep all text editable (not outlined)
- The frame should be named "Booth Spread — The Hub" at 6000×3000px

When done, confirm what was created and note the frame/page location so Alex can find it immediately.

When completely finished, run: openclaw system event --text "Done: Booth design built in Figma — Social Media Templates file, Web Summit Booth page" --mode now
