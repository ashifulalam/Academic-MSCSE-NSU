# Contributing Notes for AI and Future Updates

This file explains how this repository should be maintained.

The goal is to make the structure, writing style, and workflow clear enough that any AI tool or future helper can work in this repository without needing the same instructions again.

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

This is not a software project in the usual sense. It is mainly a document archive that should stay clean, organized, and easy to browse.

## Current Top-Level Structure

Use the current top-level structure unless the user explicitly asks for a reorganization.

- `Academic Calendar`
- `CSE534.1 Software Quality Assurance`
- `CSE583.1 Digital Image Processing`
- `Qualifying Exam`

There is also a root `README.md` that acts as the main index for the repository.

## General Principles

- Keep the repository simple, clean, and easy to scan.
- Do not make unnecessary structural changes.
- Prefer clarity over cleverness.
- Keep naming consistent.
- When changing documentation, preserve the existing tone unless the user asks for a rewrite.
- If something is already clean and correct, do not change it just to make it different.

## File Placement Rules

Place new files in the most relevant folder.

Top-level content should go into one of:

- `Academic Calendar`
- `CSE534.1 Software Quality Assurance`
- `CSE583.1 Digital Image Processing`
- `Qualifying Exam`

Inside course folders, use the most relevant subfolder such as:

- `Books`
- `My Notes`
- `Assignment`
- `Paper`
- `Project`
- `Exam`
- `Slides`

If a new kind of material does not fit the existing structure, create a clearly named new subfolder only when necessary.

## README Rules

There are two kinds of README files in this repository:

1. The root `README.md`
2. One `README.md` inside each main top-level folder

### Root README Rules

The root `README.md` is the main entry point for the repository.

It should:

- have a clean title
- have a short repository description
- include the course index table
- stay concise and easy to read

If the root README is updated, keep the style simple and structured.

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
- do not reorganize folders unless the user explicitly asks
- do not create extra README files unless asked
- keep documentation changes consistent with the existing style
- use simple wording
- use the standard course README layout for course folders
- preserve user-provided academic details exactly unless asked to rewrite them
- prefer safe, minimal, clear changes

If the user gives a direct formatting preference, follow the user's preference over older wording in the repository.

## Before Finishing Any Documentation Update

Before finishing, check the following:

- does the README match the real folder contents?
- is the wording consistent with the repository rules?
- are `Faculty` and `Office` used consistently?
- are emails inside `Contact` instead of `Course Info`?
- did you avoid adding unnecessary sections?
- does the change help future readability?

If the answer is yes to all of these, the documentation change is probably good.
