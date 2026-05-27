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

The current second-semester course folders are:

- `CSE511.1 Advanced Algorithms`
- `CSE565.1 Digital Signal Processing`

Future semester course folders may be added later. When that happens, follow the new semester branch rules below.

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
- current semester course folders
- other clearly named academic folders requested by the user

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

## New Semester Branch Rules

The user prefers a clean branch for each new semester when starting fresh.

When creating a new semester branch:

- create a semester checkpoint tag for the previous semester if the user asks
- create a clean orphan branch for the new semester when the user wants a fresh view
- keep only `RULES.md` and `.gitignore` at the start of the clean branch
- make the new semester branch the GitHub default branch if the user asks
- do not copy old semester folders into the new semester branch
- keep the old semester files safe on the previous branch
- add only the new semester course folders and current semester academic files

For branch names, use simple semester names such as:

- `second-semester`
- `third-semester`
- `fourth-semester`

For semester tags, use simple checkpoint names such as:

- `first-semester`
- `second-semester`
- `third-semester`

## Future Course and Semester Rules

The user is currently using a clean second-semester branch. More courses and semesters may be added later.

When a new course is added:

- create or update the correct course folder
- update the root `README.md` course index
- update the correct semester table in `CGPA.md`
- add a folder `README.md` only for main top-level course folders
- keep the course naming style consistent with existing course folders

When a new semester is added:

- create a clean semester branch if the user wants a fresh working directory
- keep previous semester branches unchanged unless the user asks
- do not bring old semester folders into the new clean branch unless the user asks
- keep the root `README.md` focused on the current semester

## README Rules

There are two kinds of README files in this repository:

1. The root `README.md`
2. One `README.md` inside each main top-level folder

### Root README Rules

The root `README.md` is the main entry point for the repository.

It should:

- have a clean title
- avoid extra description text unless the user asks for it
- focus on the current semester branch
- stay concise and easy to read

If the root README is updated, keep the style simple and structured.

### New Semester Root README Layout

For a clean semester branch, use this root `README.md` layout:

1. semester title
2. `Grading Policy`
3. one assessment table for each current semester course

Do not include a course index table unless the user asks for it.

Do not include a paragraph description under the title unless the user asks for it.

### Grading Policy Rules

Place `Grading Policy` near the top of the root `README.md`.

Use this table format:

- `Numerical Score`
- `Letter Grade`
- `Grade Points`

Do not include `Performance Remarks` unless the user asks for it.

Use these rows unless the user gives a different grading scale:

- `93 and above | A | 4.0`
- `90 - 92 | A- | 3.7`
- `87 - 89 | B+ | 3.3`
- `83 - 86 | B | 3.0`

### Assessment Tracking Table Rules

For each current semester course in the root `README.md`, create a separate table.

Use the course name as the section title, for example:

- `CSE511.1 Advanced Algorithms`
- `CSE565.1 Digital Signal Processing`

Each assessment table should include these columns:

- `Assessment`
- `Date`
- `Marks`
- `Lost Marks`

Each assessment table should include these rows:

- `Quiz 1`
- `Quiz 2`
- `Quiz 3`
- `Mid`
- `Final`
- `Attendance`
- `Total Lost Marks`

Use `Pending` until the user provides real dates, marks, or lost marks.

For `Total Lost Marks`, leave the empty cells blank and put `Pending` under the `Lost Marks` column.

## CGPA.md Rules

The root `CGPA.md` file is for CGPA planning and academic progress tracking.

It should:

- keep the CGPA summary near the top
- keep the grading policy inside `CGPA.md`, not the root `README.md`
- keep `Course Outcome` as the main section for course result tracking
- keep semester course tables under `Course Outcome`
- use `Pending` until real grades are available
- update `Letter Grade`, `Grade Point`, and `Decision` after results are published
- update `Current CGPA`, semester `Total CGPA`, and `Total Credit` when official grades or credits change
- calculate semester CGPA from the course grade points
- keep all CGPA and grade-result tracking inside `CGPA.md`
- keep the page simple enough to update every semester

### CGPA Update Rules

When official grades are published, update only `CGPA.md` with:

- `Current CGPA`
- `Total Credit`
- course `Letter Grade`
- course `Grade Point`
- semester `Total CGPA`
- course `Decision` only if the user gives a decision

Do not add CGPA or grade-result details to:

- root `README.md`
- course folder README files
- folder descriptions outside `CGPA.md`

### Course Outcome Rules

Use this structure inside `Course Outcome`:

- `First Semester`
- `Second Semester`
- future semester sections when new semesters are added

Each semester course table should include:

- `Course Name`
- `Term`
- `Decision`
- `Letter Grade`
- `Grade Point`

Each semester table should include a final `Total CGPA` row.

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

Current semester course folders should have their own `README.md`.

Do not automatically create README files inside every subfolder.

Do not add `README.md` inside `Academic Calendar` unless the user explicitly asks for it.

## Academic Calendar Rules

Use `Academic Calendar` for semester calendar PDF files and related official calendar documents.

- create the `Academic Calendar` folder when the user asks for it
- keep calendar PDFs inside `Academic Calendar`
- do not add a README inside `Academic Calendar` unless the user asks
- keep the original calendar file name unless the user asks to rename it

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

### Result and CGPA Rules

- Keep CGPA and grade results only inside `CGPA.md`
- Do not add `Result` sections to course folder README files
- Do not add CGPA information to the root `README.md`
- Course folder README files should stay focused on course info, contact details, office hours, and subdirectories

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
