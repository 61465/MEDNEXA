# MEDNEXA Brand Guide v1

**"Connecting Healthcare"**

---

## 1. Brand Personality

| Trait | Description |
|---|---|
| **Trustworthy** | Medical-grade seriousness. No pun logos, no cartoons. |
| **Technical** | Precise, engineering-forward. Numbers matter. |
| **Human** | Arabic-first. Egyptian identity. Warm despite technical. |
| **Institutional** | Ready to sign a 5M EGP contract. Government-approved feel. |
| **Compliant** | PDPC/GDPR/HIPAA visual cues throughout. |

**Voice:** "We connect what's already there. Silently. Securely."
**Anti-voice:** Not disruptive, not "revolutionary," not "AI-powered" (yet).

---

## 2. Logo Concept

### Wordmark: `MEDNEXA`
- **Font:** Inter (Google Fonts, opensource, medical-clean)
- **Weight:** 700 (Bold) for main mark
- **Letter-spacing:** -0.02em (slightly tight, professional)
- **Case:** UPPERCASE

### Icon: The "N-Link"
Two circles connected by a diagonal stroke forming a stylized "N" — represents the integration between two systems.

```
 O ─╲
     ╲ O
      ╲
   MEDNEXA
```

**Interpretation:** Left circle = source system (device/HIS). Right circle = destination (records/portal). Stroke = MEDNEXA the connector.

### Full Logo Layouts
- **Horizontal:** [N-Link icon] MEDNEXA
- **Stacked:** [N-Link icon]<br/>MEDNEXA<br/>Connecting Healthcare
- **Icon only:** For favicon, app icon, watermark
- **Wordmark only:** For narrow contexts

---

## 3. Color System

### Primary Palette

| Name | HEX | RGB | Usage |
|---|---|---|---|
| **MEDNEXA Navy** | `#0A2540` | 10, 37, 64 | Primary background, headers |
| **MEDNEXA Teal** | `#00B4A6` | 0, 180, 166 | Accent, CTAs, links |
| **Clinical White** | `#FAFBFC` | 250, 251, 252 | Text on dark, cards |
| **Trust Blue** | `#1E88E5` | 30, 136, 229 | Secondary CTA, informational |

### Neutral Palette

| Name | HEX | Usage |
|---|---|---|
| Slate 900 | `#0F172A` | Body text on light |
| Slate 600 | `#475569` | Secondary text |
| Slate 300 | `#CBD5E1` | Borders, dividers |
| Slate 100 | `#F1F5F9` | Light backgrounds |

### Semantic Palette

| Name | HEX | Usage |
|---|---|---|
| Success Green | `#10B981` | Compliant/Success states |
| Warning Amber | `#F59E0B` | Compliance warnings |
| Error Red | `#EF4444` | Errors, breach alerts |
| Info Cyan | `#06B6D4` | Info messages |

### Accessibility
- Body text (Slate 900 on Clinical White): contrast 15.2:1 ✅
- Teal on Navy: contrast 4.7:1 ✅ (WCAG AA)
- All CTAs must maintain 4.5:1 contrast minimum

---

## 4. Typography

### Font Stack

**Primary (Latin + Numbers):**
```css
font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
```

**Arabic Primary:**
```css
font-family: 'IBM Plex Sans Arabic', 'Cairo', 'Noto Sans Arabic', sans-serif;
```

Both are Google Fonts / free-license.

### Type Scale

| Element | Size | Weight | Line-Height |
|---|---|---|---|
| Display XL | 72px | 800 | 1.05 |
| Display L | 60px | 700 | 1.1 |
| H1 | 48px | 700 | 1.15 |
| H2 | 36px | 700 | 1.2 |
| H3 | 24px | 600 | 1.3 |
| Body L | 18px | 400 | 1.6 |
| Body | 16px | 400 | 1.6 |
| Body S | 14px | 400 | 1.5 |
| Caption | 12px | 500 | 1.4 |

---

## 5. Iconography

Use **Lucide Icons** (opensource, MIT). Preferred set:
- `activity` — Health metrics
- `shield-check` — Compliance
- `link-2` — Integration
- `database` — Data storage
- `stethoscope` — Clinical
- `layers` — Architecture
- `zap` — Performance

**Style rules:**
- Stroke width: 1.5px
- No fills unless in badges
- Match text color

---

## 6. Iconography — Clinical Trust Signals

Badges to display on landing page:
- `DICOM Conformant`
- `HL7 v2.5 Compliant`
- `FHIR R4 Ready`
- `PDPC Aligned (Law 151/2020)`
- `ISO 27001 Roadmap`

---

## 7. Imagery Direction

**Do:**
- Real Egyptian hospital environments (with permission)
- Diverse healthcare workers (age, gender, role)
- Technology in context (screens, devices, networks)
- Warm, natural lighting

**Don't:**
- Stock photos of white doctors in blue scrubs
- AI-generated hospital images (uncanny)
- Overly clinical/sterile shots
- Cliché stethoscope-on-keyboard

**Photography palette:** Slightly desaturated, warm midtones, teal accents in post.

---

## 8. Voice & Copy

### Do
- "Integration you can audit."
- "Compliant by design."
- "Connect. Secure. Comply."
- "Built for the mid-market Egyptian hospital."

### Don't
- "Revolutionary AI-powered platform"
- "The future of healthcare"
- "Disrupting the industry"

### Arabic Tone
- Modern Standard Arabic (فصحى معاصرة)
- Avoid slang, avoid overly formal legal register
- Technical terms in English where standard (DICOM, HL7, PACS, RIS) with Arabic gloss on first use

---

## 9. Applications

### Business Cards
Navy background, Teal N-Link icon, Clinical White text.

### Slide Master
- Cover: Navy full-bleed, Teal N-Link, wordmark below
- Section dividers: Navy with white type
- Content: White with Navy H1s, Slate 900 body
- Data slides: Grid on Slate 100 with Teal accent

### Email Signature
```
[Name]
[Role] | MEDNEXA
+20 XXX XXX XXXX | name@mednexa.co
mednexa.co · "Connecting Healthcare"
```

---

## 10. Do-Not-Use Zone

- No emoji in any professional context
- No AI-generated art in customer-facing materials
- No stock icons of syringes / red crosses / caduceus (over-used clichés)
- No purple/pink (feminine tech connotation not aligned with institutional)
- No green as primary (medical context but too "startup")
