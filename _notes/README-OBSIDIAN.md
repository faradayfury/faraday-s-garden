---
title: Obsidian Setup Instructions
date: 2024-12-19
---

## 🧠 Obsidian Digital Garden Setup

This folder is configured to work as an Obsidian vault for your Jekyll digital garden.

## How to Use

#### 1. Open this folder as an Obsidian vault

- In Obsidian, click "Open folder as vault"
- Select this `_notes` folder
- Obsidian will automatically load the configured settings

#### 2. Creating New Notes

- Use Cmd+N (Mac) or Ctrl+N (Windows) to create a new note
- New notes will automatically get Jekyll front matter
- All new notes will appear on your website's index page automatically

#### 3. Editing Existing Notes

- Click on any `.md` file to edit
- Changes are automatically saved
- Your Jekyll site will reflect changes when you rebuild

#### 4. File Organization

- You can create subfolders (like `animals/`) for organization
- Jekyll will still find and index all notes regardless of folder structure

## Important Notes

- **Front Matter Required**: Each note needs the `---` front matter block at the top
- **Automatic Indexing**: Your Jekyll site automatically shows all notes on the index page, sorted by last modified date
- **Markdown Links**: This vault is configured to use standard markdown links `[text](link)` instead of wiki links for Jekyll compatibility

## Website Integration

Your notes automatically appear on your website at:

- Individual notes: `yoursite.com/note-title`
- Index page: `yoursite.com/` (shows all notes chronologically)

Happy writing! 🚀
