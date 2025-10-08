# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This repository contains course schedule documentation for the MSBA (Master of Science in Business Analytics) cohort at the Gies College of Business, University of Illinois, Fall 2025 semester.

**Primary audience**: Students, teaching assistants, and faculty coordinating a cohort of ~90 students taking 3 mandatory courses and 1 elective course simultaneously.

## Repository Structure

### Source Materials
The repository contains PDF and DOCX files with official course schedules:
- `badm554-schedule-fall2025.pdf` - Enterprise Database Management (mandatory, 4 credits)
- `BDI513 weekly plan FA25.pdf/docx` - Data Storytelling (mandatory, 4 credits)
- `BusinessIntelligence_BADM 557_WeeklyPlan (1).pdf/docx` - Business Intelligence (elective, 2-4 credits, ~45 students)
- `fin 550 course_plan.pdf/xlsx` - Big Data Analytics in Finance (mandatory, 4 credits)

### Generated Artifacts
- `weekly-synthesis.md` - **Primary output**: Week-by-week synthesis table showing all courses side-by-side across the 16-week semester

## Key Concepts

### Course Information Context
- **Cohort size**: 90 students (all take 3 mandatory courses, ~50% take BADM 557 elective)
- **Semester length**: 16 weeks (Aug 25 - Dec 12, 2025)
- **Common elements across courses**:
  - Machine learning techniques (regression, classification)
  - Case-based learning
  - Final projects due in Week 15-16

### Tools & Technology Stack by Course

**BADM 554 (Database Management)**:
- SQL (primary language)
- Jupyter notebooks
- Minimal Python usage
- MySQL Workbench (ER modeling)
- Knime (ETL)
- MongoDB (NoSQL)
- DataCamp for assignments

**BDI 513 (Data Storytelling)**:
- Wolfram notebooks (primary environment)
- Tableau
- Python for some analyses
- Financial data APIs (Nasdaq datalink, Yelp API)
- Bloomberg Terminal (Excel add-in)

**FIN 550 (Finance Analytics)**:
- R (primary language)
- RStudio
- Cloud computing platforms
- ISLR textbook (Introduction to Statistical Learning with R)

**BADM 557 (Business Intelligence)**:
- Python (Scipy, Numpy, Pandas, Scikit-learn)
- Tableau
- Python certification requirement
- Various data sources (10K filings, Mergent, Moody's, CapitalIQ, S&P)

### Analysis Focus Areas
When working with this data, consider:
1. **Workload clustering**: Identify weeks where multiple assessments/projects overlap
2. **Topic overlap**: Find redundancies in content (e.g., regression taught in 3+ courses)
3. **Skill progression**: Track how technical skills build from foundational to advanced
4. **Practicum integration**: Most students also do client-facing practicum work

## Common Tasks

### Adding New Course Schedules
When new semester schedules are added:
1. Place PDF/DOCX files in root directory
2. Update `weekly-synthesis.md` to reflect new dates/content
3. Commit with descriptive message following the existing commit format

### Generating Analysis
To create week-by-week synthesis:
1. Read all course schedule PDFs/documents
2. Extract weekly topics, assignments, and due dates
3. Create markdown table with columns: Week | Dates | [Course 1] | [Course 2] | [Course 3] | [Course 4]
4. Add analysis sections for workload patterns, overlaps, and skill progression

### Updating Synthesis
When course schedules change:
1. Identify which course(s) changed
2. Update only affected rows in the weekly-synthesis.md table
3. Review "Key Observations" section for accuracy
4. Commit with clear description of what changed

## Content Guidelines

### Synthesizing Course Content
- Use **bold** for major assessments (exams, project due dates)
- Include assignment identifiers (Quiz 1, H1, Lab 4, etc.)
- Note class cancellations explicitly
- Preserve course-specific terminology (e.g., "Share & Tell" for BADM 557)

### Analysis Sections
The synthesis document includes:
- **Heavy Workload Weeks**: Periods with multiple assessments across courses
- **Topic Overlap by Week**: When 2+ courses cover similar content
- **Assessment Clusters**: Weeks with high due date density
- **Skill Development Timeline**: Semester-long progression from foundations → advanced topics

## Git Workflow

This repository uses standard git workflow:
```bash
git add [files]
git commit -m "Descriptive message"
git push origin main
```

Commit messages should follow the established pattern:
- Start with verb (Add, Update, Fix)
- Include course codes when relevant
- Add collaborative attribution footer for AI-generated content
