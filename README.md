# PlanSentinel 🚧🤖
**AI pre-checker for plan PDFs.**  
Detects missing **north arrow**, **scale bar**, **title block**, **grid tags**, and **section markers**. Then generates a clean **Issues Report**.

Goal: catch common, expensive drawing omissions before review/permit/submittal.

---

## What it does (v0)
Input: a plan PDF (one or multiple pages)

Output:
- Annotated page images (detections drawn on the sheet)
- detections.json (all detections with confidence + bounding boxes)
- issues_report.json + issues_report.md (human-readable checklist)

### Detected classes (v0)
- `north_arrow`
- `scale_bar`
- `title_block`
- `grid_bubble`
- `section_marker`


## Why this matters
Missing or inconsistent sheet elements cause confusion, RFIs, rework, and delays.
PlanSentinel is a pre-check: fast feedback for teams before sharing drawings.

## Limitations
This is a pre-check, not a final engineering review.
Detection quality depends on sheet resolution, scanning artifacts, and drawing style.
No client/confidential drawings should be uploaded to this repo.

---

## Contact
Built by **Jerónimo Rodríguez**  
j.rodriguezj2@uniandes.edu.co
Jerorodrijim@gmail.com

