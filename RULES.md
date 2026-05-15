# AI Rules and Project Guide

This file is the main instruction guide for any AI tool working in this repository.

Read this file first before editing, reorganizing, committing, or suggesting changes.

These rules apply to any AI helper, including Codex, Claude, Gemini, ChatGPT, or any other tool.

The goal is to make the project clear enough that the user does not need to explain the same structure, naming style, commit style, or documentation rules again.

## First Things an AI Must Do

Before making changes, an AI should:

- read this `RULES.md` file
- check the current repository structure
- check the files related to the user's request
- preserve the existing organization unless the user asks for a change
- make the smallest clear change that solves the request
- explain important changes in simple language

Do not assume this is a software project.

## Repository Purpose

This repository is a personal academic archive for an MScSE journey at North South University.

It contains:

- course materials
- personal notes
- books
- slides
- papers
- project files
- academic calendar files
- qualifying exam resources

This is mainly a document archive that should stay clean, organized, and easy to browse.

The repository should help the user:

- find course materials quickly
- track courses by semester
- keep faculty and contact information organized
- track CGPA planning and course outcomes
- keep future semester additions consistent
- maintain clean Git history with easy commit messages

## Important Root Files

These root files have special meaning:

- `README.md` is the main public index of the repository
- `CGPA.md` is for CGPA planning, grade targets, and semester course outcomes
- `RULES.md` is the instruction file for AI tools and future updates
- `.gitignore` keeps temporary files out of Git

## Current Top-Level Structure

Use the current top-level structure unless the user explicitly asks for a reorganization.

- `Academic Calendar`
- `CSE534.1 Software Quality Assurance`
- `CSE583.1 Digital Image Processing`
- `Qualifying Exam`

The current first-semester course folders are:

- `CSE534.1 Software Quality Assurance`
- `CSE583.1 Digital Image Processing`

Future semester course folders may be added later. When that happens, update the related index and tracking files instead of changing the whole structure.

## General Principles

- Keep the repository simple, clean, and easy to scan.
- Do not make unnecessary structural changes.
- Prefer clarity over cleverness.
- Keep naming consistent.
- When changing documentation, preserve the existing tone unless the user asks for a rewrite.
- If something is already clean and correct, do not change it just to make it different.

## File Placement Rules

Place new files in the most relevant folder.

Root-level files should be used only for repository-wide information.

Use root-level files this way:

- use `README.md` for the main course index
- use `CGPA.md` for CGPA planning and course outcome tracking
- use `RULES.md` for AI instructions and repository workflow rules
- use `.gitignore` for ignored temporary files

Top-level content should go into one of:

- `Academic Calendar`
- `CSE534.1 Software Quality Assurance`
- `CSE583.1 Digital Image Processing`
- `Qualifying Exam`

Do not put course-specific books, slides, notes, papers, exams, or projects directly in the repository root.

Inside course folders, use the most relevant subfolder such as:

- `Books`
- `My Notes`
- `Assignment`
- `Paper`
- `Project`
- `Exam`
- `Slides`

If a new kind of material does not fit the existing structure, create a clearly named new subfolder only when necessary.

## Future Course and Semester Rules

The user is currently in the first semester. More courses and semesters will be added later.

When a new course is added:

- create or update the correct course folder
- update the root `README.md` course index
- update the correct semester table in `CGPA.md`
- add a folder `README.md` only for main top-level course folders
- keep the course naming style consistent with existing course folders

When a new semester is added:

- add a new semester section in `CGPA.md`
- keep previous semester sections unchanged unless the user asks
- do not reorganize old courses into new semester folders unless the user explicitly asks
- keep the root `README.md` simple and easy to scan

## README Rules

There are two kinds of README files in this repository:

1. The root `README.md`
2. One `README.md` inside each main top-level folder

### Root README Rules

The root `README.md` is the main entry point for the repository.

It should:

- have a clean title
- optionally have a short repository description if the user wants one
- include the course index table
- stay concise and easy to read

If the root README is updated, keep the style simple and structured.

## CGPA.md Rules

The root `CGPA.md` file is for CGPA planning and academic progress tracking.

It should:

- keep the CGPA summary near the top
- keep the grading policy inside `CGPA.md`, not the root `README.md`
- keep `Course Outcome` as the main section for course result tracking
- keep semester course tables under `Course Outcome`
- use `Pending` until real grades are available
- update `Letter Grade`, `Grade Point`, and `Decision` after results are published
- calculate semester CGPA from the course grade points
- keep the page simple enough to update every semester

### Course Outcome Rules

Use this structure inside `Course Outcome`:

- `First Semester Courses`
- `Second Semester Courses`
- future semester sections when new semesters are added

Each semester course table should include:

- `Course Name`
- `Term`
- `Letter Grade`
- `Grade Point`
- `Decision`

Use the same decision labels unless the user asks for a change:

- `✅ Satisfied`
- `🙂 Average`
- `⚠️ Below Average`
- `❌ Not Satisfied`
- `🔁 Retake`
- `🗑️ Discard`

When a new course is added, update both:

- root `README.md` course index
- the correct semester table in `CGPA.md`

When a new semester starts, add a new semester section in `CGPA.md` only when the user asks or when course details are available.

### Top-Level Folder README Rules

Only the main top-level folders should have their own `README.md`, unless the user explicitly asks for more nested README files.

At the moment, these folders should have README files:

- `Academic Calendar`
- `CSE534.1 Software Quality Assurance`
- `CSE583.1 Digital Image Processing`
- `Qualifying Exam`

Do not automatically create README files inside every subfolder.

## Standard Course README Layout

For course folders, use this section order:

1. `Course Info`
2. `Contact`
3. `Office Hours` when needed
4. `Subdirectories`

### Course Info Rules

Inside `Course Info`, keep these fields:

- `Term`
- `Semester`
- `Faculty`
- `Office`

### Contact Rules

- Put email addresses inside `Contact`
- Do not put email addresses inside `Course Info`
- If a faculty member has more than one email, keep all important ones

### Office Hours Rules

- Only include `Office Hours` when those details are available and relevant
- If there is no office hour information, do not add an empty section

### Subdirectories Rules

- Briefly explain the purpose of each important subfolder
- Keep descriptions short and practical

## Naming Conventions

Follow these naming rules consistently:

- Use `Faculty` everywhere, not `Faculty Name`
- Use `Office` everywhere, not `Room`
- Use the same wording style across course folder README files
- Keep commit titles short, clear, and easy to understand

## Commit Rules

This repository uses simple, readable commits.

Future AI tools should follow the exact commit style below unless the user explicitly asks for a different style.

### Commit Title Format

Use this pattern for commit titles:

- `Add ...`
- `Update ...`
- `Rename ...`
- `Remove ...`
- `Clean ...`

The title should:

- start with a clear action word
- be short and easy to understand
- say exactly what changed
- use normal words
- avoid vague wording

Good examples:

- `Add books for CSE534`
- `Add README for CSE583 course folder`
- `Add lecture slides for CSE583`
- `Update main README course table`
- `Update course README layout`
- `Rename README title`
- `Add gitignore and clean temp files`
- `Add AI workflow notes`

Bad examples:

- `Update files`
- `Fix stuff`
- `Misc changes`
- `Changes`
- `Small update`

### Commit Body Format

The commit body must follow these rules:

- use bullet points only
- each bullet should describe one actual change in that commit
- mention only what is included in that commit
- keep each bullet short and direct
- use simple language
- do not add background story or unnecessary explanation

Use lowercase wording inside the bullet points unless a proper name needs capital letters.

Good examples:

- `add the main textbook for Digital Image Processing`
- `add final, midterm, and math solution files for exam preparation`
- `change the CSE534 README to use Course Info and Contact sections`
- `define README layout rules for course folders`

Bad examples:

- `this commit improves many things in the repo`
- `worked on several updates`
- `made some changes to keep things better`

### Commit Message Template

Use this exact shape for commit messages:

```text
Commit title

- explain one clear change
- explain another clear change
- mention only what this commit includes
```

Example:

```text
Update CGPA tracking rules

- add rules for CGPA semester tables
- define course outcome decision labels
- explain when to update CGPA.md
```

### Recommended Commit Titles by Change Type

Use these examples as a guide when choosing commit titles:

- `Add CGPA planning page`
- `Add README for CSE534 course folder`
- `Add CSE534 lecture slides`
- `Add books for CSE583`
- `Update main README course index`
- `Update CGPA course outcomes`
- `Update AI workflow rules`
- `Update course README details`
- `Rename contributing guide to rules`
- `Remove unused README section`
- `Clean temporary files`

### Commit Scope Rules

- Prefer one commit for one main topic
- Do not mix unrelated changes in the same commit
- Keep related files together only when they belong to the same clear topic
- If a README change directly explains files added in the same topic, it can be committed together
- If the change covers a different topic, use a separate commit

### Folder-by-Folder Commit Pattern

When adding a course folder in a clean sequence, use this pattern when practical:

1. top `README.md`
2. course folder `README.md`
3. `Books`
4. `My Notes` or `Assignment`
5. `Paper`
6. `Project`
7. `Exam`
8. `Slides`

Use the closest matching version of this pattern depending on the actual folder structure.

### Commit Checklist

Before making a commit, check:

- is the commit about one clear topic?
- does the title clearly say what changed?
- does the body use only bullet points?
- does the body mention only the files or documentation changed in this commit?
- would someone understand the commit from the title and bullets alone?

## When to Update READMEs

Update the root `README.md` when:

- a new course is added
- the course table changes
- the title changes
- the repository description changes

Update `CGPA.md` when:

- a new course is added
- a new semester starts
- grades are published
- grade points change
- course decisions change
- CGPA summary changes

Update a folder `README.md` when:

- a new important subfolder is added
- faculty details change
- office details change
- contact details change
- office hours are added or changed
- file locations change in a meaningful way
- the folder structure changes enough that the README would become outdated

## Cleanup Rules

Keep the repository free of temporary files and metadata files.

- Do not keep `.DS_Store` files
- Do not keep temporary Office files such as `~$...`
- Keep `.gitignore` updated if similar junk files appear

## AI Agent Behavior Rules

Any AI tool working in this repository should follow these rules:

- read the current repository structure before making assumptions
- check `README.md`, `CGPA.md`, and relevant folder README files before editing academic documentation
- do not reorganize folders unless the user explicitly asks
- do not create extra README files unless asked
- keep documentation changes consistent with the existing style
- use simple wording
- use the standard course README layout for course folders
- preserve user-provided academic details exactly unless asked to rewrite them
- prefer safe, minimal, clear changes

If the user gives a direct formatting preference, follow the user's preference over older wording in the repository.

## What AI Tools Should Not Do

Avoid these actions unless the user clearly asks for them:

- do not rename major folders
- do not move course folders into semester folders
- do not remove academic files
- do not delete or rewrite user-provided faculty information
- do not add unnecessary nested README files
- do not add complex formatting that makes Markdown hard to maintain
- do not mix unrelated topics in one commit
- do not use vague commit messages

## Before Finishing Any Documentation Update

Before finishing, check the following:

- does the README match the real folder contents?
- is the wording consistent with the repository rules?
- are `Faculty` and `Office` used consistently?
- are emails inside `Contact` instead of `Course Info`?
- did you avoid adding unnecessary sections?
- does the change help future readability?

If the answer is yes to all of these, the documentation change is probably good.
