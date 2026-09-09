# Term 2 — MBA 2026-28

## Folder structure

```
Term_2/
├── _sources/                     # Reference material, not day-to-day notes
│   ├── Course_Outlines/          # All syllabi as PDF: <Course>_Outline.pdf
│   ├── Cases/                    # One subfolder per course
│   │   └── <Course>/
│   │       ├── _Cases_Index.md          # links to every case in the course
│   │       ├── <Course>_Coursepack.docx # the official case/article list
│   │       ├── <Case_Name>.md           # case reference: source, synopsis, facts
│   │       └── <Case_Name>_Notes.md     # Quick read + your class notes
│   └── Extra_Materials/          # Readings, articles, textbooks — one subfolder per course
│       └── <Course>/
│
├── <Course>/                     # One folder per course (see list below)
│   ├── Lecture_1.md              # Lecture notes live directly in the course folder
│   ├── Lecture_2.md
│   └── Slides/                   # Lecture decks (pdf/pptx) — the only subfolder
│
├── _templates/
│   └── Lecture_Note.md           # Copy into a course folder when starting a lecture
│
└── README.md
```

## Courses

| Folder | Course |
|---|---|
| `Communication_II` | Communication II |
| `Corporate_Finance` | Corporate Finance |
| `Entrepreneurship` | Entrepreneurship / The Entrepreneurial Manager |
| `Macroeconomics` | Macroeconomics |
| `Macro_Organizational_Behavior` | Macro Organizational Behavior (Macro-OB) |
| `Managerial_Accounting` | Managerial Accounting |
| `Marketing_Management_II` | Marketing Management II |
| `Operations_Management_I` | Operations Management I |

## Conventions

- **Naming:** `snake_case`, underscores instead of spaces (`Corporate_Finance`, `Lecture_3.md`).
- **A course folder contains only lecture-note `.md` files and a `Slides/` subfolder.** Nothing else.
- **Lecture notes:** one file per session, numbered — `Lecture_1.md`, `Lecture_2.md` — sitting directly in the course folder. Start from `_templates/Lecture_Note.md`.
- **Course outlines** live only in `_sources/Course_Outlines/`, all as PDF — don't duplicate them into course folders.
- **Cases & coursepacks** live in `_sources/Cases/<Course>/`. Each case has two markdown files: `<Case_Name>.md` (source link, product ID, synopsis, facts, decision) and `<Case_Name>_Notes.md` (a **Quick read** blockquote for the 30-second gist, then a **Notes** skeleton for class prep). `_Cases_Index.md` lists them all. Drop the actual case PDFs here too once downloaded from Moodle. Synopses were written from public knowledge — verify against the real case text; anything unverifiable is marked `_Complete after reading._`.
- **Macroeconomics** has no formal cases — its coursepack is all articles/data/news, so it has no case files.
- **Slides** go in `<Course>/Slides/`, named `Lecture_1_slides.pdf` etc. to line up with the notes.
- `_sources/` and `_templates/` sort to the top because of the leading underscore.
- `.gitkeep` files keep empty folders under version control — delete one once the folder has real content.
