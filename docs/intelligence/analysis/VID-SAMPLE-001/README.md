# Analysis Report — VID-SAMPLE-001

**Source:** [VID-SAMPLE-001](../../sources/VID-SAMPLE-001.md)  
**Captured:** 2026-08-20  
**Analyst notes:** Phase-2 sample for Instagram Reel pipeline

## 1. Source Summary

Short Instagram Reel teaching a nested corner-radius formula for consistent UI containers. Caption leads with “Stop guessing your corner radius” and a lead-magnet CTA (“Comment CORNER…”). Same teaching point appears on LinkedIn with an explicit transcript and on YouTube (Memorisely, 16s).

## 2. Creator Profile

See source profile. Educator / design-craft content. Credibility B for craft heuristics; not a standards body.

## 3. Capture limitations

| Layer | Status |
| --- | --- |
| Caption / metadata | ✅ complete |
| Speech transcript | ✅ via LinkedIn cross-post (same script) |
| Full video frames / UI overlays | ⚠️ partial — cover frame only; demo UI not frame-captured |
| Audio file | ❌ not stored |

Treat SpeechVsVisual as **partial** until a frame dump exists.

---

## 4. Layer 1 — Transcription (speech)

Source: LinkedIn transcript of the same tip (aligned with Reel caption/hook).

> Not guessing your corner radius. Let's assume you've got this card and you're trying to get the corner radius right? Well, instead of guessing, you can follow this method. Most designers when they're setting corner radius, focus on the inner and then apply the same radius to the outer. But this creates this really awkward gap. So instead use your inner plus the padding to equal the outer radius. You can see what it looks like across tight regular and then loose fitting super.

### Marked claims

| # | Type | Text |
| --- | --- | --- |
| C1 | Recommendation | Use **Inner + Padding = Outer** for nested corner radii |
| C2 | Anti-pattern / Assertion | Applying the **same** radius to inner and outer creates an awkward gap |
| C3 | Example | Works across tight / regular / loose padding |
| C4 | Justification (implied) | Removes guessing; improves visual consistency for teams |
| C5 | Caveat (audience comment, not creator) | Corner smoothing (squircle %) and non-equal H/V padding complicate the simple formula |

Caption-only claims:

| # | Type | Text |
| --- | --- | --- |
| C6 | Workflow / Marketing | Comment CORNER for DM with “go to radius options” (personal token set — not captured) |
| C7 | Goal statement | Helps design teams keep things clean and consistent |

---

## 5. Layer 2 — Visual analysis

### Cover frame (`assets/cover.jpg`)

- Hook overlay text: **“Stop guessing your corner radius”**
- Creator on camera (beanie, pointing gesture); designer keyboard (Work Louder, per caption)
- No nested-card UI visible on cover — instructional face-to-camera hook

### Demo UI (from speech + cross-source restatements; **not** independently frame-verified here)

Expected shown content (verify later with frames):

- Nested card/container with padding
- Wrong state: identical inner/outer radius → uneven concentric gap (“pregnant” corners — community language)
- Right state: outer = inner + padding
- Variants: tight / regular / loose padding

**SpeechVsVisual:** `partial` — speech clear; visual demo not fully captured in this repo yet.

---

## 6. Key Insights

1. Tip encodes a **geometric consistency principle** for nested radii, not accessibility.
2. Strong pedagogical anti-pattern (same radius nested) makes the rule AI-teachable.
3. CTA hides the creator’s concrete radius scale → we must **not** invent token values from this Reel.
4. Commenter raises real exceptions (smoothing, asymmetric padding) → document as Exceptions, don’t ignore.

## 7. Extracted Principles (candidates)

See `claims.md` and `principles/PRINCIPLE-RADIUS-001.md`.

## 8. Design Rules

None promoted to Canonical/CORE from this source alone.

## 9. Visual Observations

- Social format: hook text + talking head; formula likely on-screen in later frames (unverified).
- Production quality high; engagement ~72k likes — **not** evidence quality.

## 10. UX Insights

- Nested surface consistency reduces visual noise (related to hierarchy / craft, P5).
- Does not change interaction, IA, or feedback behavior.

## 11. Accessibility Insights

- None direct. Radius choice is not a WCAG success criterion.
- Do not let this tip override focus visibility, target size, or contrast rules (P0).

## 12. Anti-Patterns (from source)

```text
Anti-pattern:
Nested containers share the same corner radius as their parent
while padding > 0, producing uneven concentric corners / awkward gaps.

Why (per creator):
Creates a visual gap that looks inconsistent / “wrong.”
```

## 13. Confidence Scores

| Claim | Confidence | Why |
| --- | --- | --- |
| C1 formula as useful Practice | Medium | Repeated across creator channels + community articles/plugins |
| C1 as universal CORE token law | Low | Single educator lineage; systems use varied radius scales; exceptions exist |
| C2 anti-pattern | Medium | Widely restated; visually intuitive |
| Specific px token set | n/a | Not disclosed in public caption/transcript |

## 14. Source Evidence

- Instagram Reel DRuEeIPCH7M
- LinkedIn post transcript (same tip)
- Memorisely YouTube short `09T1XTD1FvI` (aligned formula)
- Community: Medium “consistent corner radius system”; Figma “Corner Perfector” plugin docs restating R_inner = R_outer − padding

## 15. Potential Skill Candidates (later)

- `spacing-radius-nesting` (Foundations) — only after cross-source with ≥1 design-system doc or multiple independent practitioners **and** Quality Gate
- Related: card nesting / surface composition skills

**Maturity now:** Observation → Principle candidate **EXPERIMENTAL**
