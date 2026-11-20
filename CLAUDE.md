# Geometry & Algebra Assistant — Standing Rules

Rules for helping a Geometry / Algebra 1 teacher (periods 1st, 3rd, 4th, 5th).
Student data is private: deliver results as downloadable files only. Never commit
gradebook CSVs, student names, or scores to this repository.

## How to read a request

1. **"Calculate students' assignment grade(s) for a unit"** (or similar):
   - If the teacher has NOT said the unit's total points, ask for the total first.
   - Once the total is known, ask for the gradebook spreadsheets (one CSV per period).
   - Then compute grades with the Unit Grading rules below.
2. **CSV gradebook files uploaded with no other instruction:** assume the teacher wants
   the **who's-behind list** (format below) and ask which assignments if not stated.

## Unit Grading rules

- Items: every lesson practice in the unit + the BETTER of the two practice tests.
  Each item is worth (unit total ÷ number of items) points. Example: 6 lessons + 1
  practice test = 7 items, total 70 → 10 points each.
- Condition 1 (Option A): sum of the lesson practices + the better practice test,
  each scaled to its point value.
- Condition 2 (Option B): better practice-test percent × unit total.
- Final score = the larger of A and B, rounded to the nearest whole number
  (halves round up). Report only the number (e.g. 50), not "50/70" or a percent.
- Blank scores ("-" or empty) count as 0. Ignore the unit test, review assignments
  (e.g. "Missed Q's Review"), and anything outside the unit.
- If a lesson appears twice in one period (duplicate/re-posted column), use the
  better of the two scores.
- Keep names exactly as exported ("Last, First").
- Deliverables: one .xlsx with a tab per period (two columns: Student, Unit N Score)
  plus one CSV per period for Google Sheets import.

## Who's-behind list (default for uploaded CSVs)

- Flag a student if their score on the assignment is below 80% OR blank.
- Word document (python-docx), Arial, Normal 20 pt. Per period: bold 24 pt black
  period heading; for each assignment a bold + underlined label ending in ":" in that
  assignment's color, then a comma-separated names line in the same color.
  First names only, sorted, de-duplicated; add a last initial when two students in
  the same period share a first name. Blank line between periods.
- Keep one color per assignment and reuse it across days.
- If an assignment is mostly or entirely blank (not yet due), point this out.
- Retake-review sections show the criterion line ("If you scored below a 70% on the
  Unit N Test") instead of names.

## General

- Build files in the session scratchpad, render a preview, and check it before
  delivering. Never overwrite an earlier deliverable; save a new version instead.
- Algebra 1 worksheets use the boxed "house format" with formula templates and an
  answer key in red; no standards labels.
