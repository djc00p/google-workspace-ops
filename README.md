# 📄 Google Workspace Ops

[![ClawHub Skill](https://img.shields.io/badge/ClawHub-Skill-blue)](https://clawhub.ai/djc00p/google-workspace-ops) [![Agent Skill](https://img.shields.io/badge/Agent-Skill-blue)](#) [![Google Workspace](https://img.shields.io/badge/Google-Workspace-4285F4.svg)](https://workspace.google.com) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Google Workspace Ops** operates Google Drive, Docs, Sheets, and Slides as a unified workflow system — find, summarize, edit, migrate, and clean up shared documents.

The hard part of shared-document work isn't editing a file. It's knowing **which** file is canonical when there are three versions, and not breaking the one your team actually relies on. This skill front-loads discovery and inspection so edits land in the right place.

---

## 🎯 When to Use

* Finding and updating a doc in place
* Consolidating plans, trackers, or notes across files
* Cleaning or restructuring a shared spreadsheet
* Importing, repairing, or reformatting slides
* Summarizing Docs, Sheets, or Slides for decisions

---

## 🔄 The Four-Step Workflow

### Step 1 — Find the Asset

Start with Google Drive search to locate:

* The exact file
* **Sibling or duplicate assets**
* Recently modified versions

Confirm by title, owner, modified time, or folder.

### Step 2 — Inspect Before Editing

Summarize the current structure:

* Tabs, headings, slide count
* Whether the task is cleanup or structural surgery
* **Pick the smallest tool that works safely**

### Step 3 — Edit with Precision

* **Docs** — use index-aware edits, not vague rewrites
* **Sheets** — operate on explicit tabs and ranges
* **Slides** — distinguish content edits from layout/template changes

> Iterate with **inspect → verify** rather than one blind update.

### Step 4 — Keep Systems Clean

Surface as part of the work:

* Duplicate trackers or decks
* Stale vs. canonical docs
* Archive/merge candidates

---

## 📋 Output Format

```text
ASSET: [name, type, why this one]
CURRENT STATE: [structure, key problems]
ACTION: [edits made or recommended]
FOLLOW-UPS: [archive, merge, clean, next steps]
```

---

## ✅ Good Use Cases

* *"Find the active planning doc and condense it"*
* *"Clean up the customer spreadsheet and show churn-risk rows"*
* *"Import this deck into Slides and make it presentable"*
* *"Find the current tracker, not the stale duplicate"*

---

## 🔐 Setup

Requires `GOOGLE_APPLICATION_CREDENTIALS` pointing at a service-account credentials file with access to the target Drive.

---

## 📚 References

* `references/drive-operations.md` — Drive search, file metadata, and duplication detection
* `references/docs-sheets-slides.md` — format-specific edit patterns

---

**Adapted from [everything-claude-code](https://github.com/affanm/everything-claude-code) by [@affaan-m](https://github.com/affaan-m) (MIT).**

**Published by [@djc00p](https://github.com/djc00p)**
