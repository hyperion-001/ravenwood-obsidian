# Ravenwood Workflow Guide

This guide explains how to use the integrated workflow between Obsidian, VSCode, and GitHub for managing your Ravenwood content.

## Setup Overview

We've set up the following:

1. Your Obsidian vault's Ravenwood folder is now a Git repository
2. This repository is connected to GitHub at: https://github.com/hyperion-001/ravenwood-obsidian.git
3. A VSCode workspace has been created that directly opens your Obsidian vault

## Workflow: Editing Files

### In Obsidian

- Continue using Obsidian as you normally would
- All changes you make in Obsidian will be visible in the Git repository
- You can use Obsidian's features for note-taking, linking, and visualization

### In VSCode

1. Open VSCode
2. Open the workspace file: `/Users/jonathanwomack/Documents/ravenwood-obsidian.code-workspace`
3. Browse and edit files directly in VSCode
4. Use VSCode's superior code editing features for RAG documents and code blocks

## Workflow: Committing to GitHub

When you want to save your changes to GitHub:

1. In VSCode, open the Source Control panel (Ctrl+Shift+G or Cmd+Shift+G)
2. Review your changes
3. Stage the files you want to commit (click the + icon next to each file)
4. Enter a commit message describing your changes
5. Click the checkmark to commit
6. Click the "..." menu and select "Push" to send changes to GitHub

## Recommended VSCode Extensions

For the best Markdown editing experience in VSCode:

- **Markdown All in One**: Keyboard shortcuts, table of contents, auto-preview
- **Markdown Preview Enhanced**: Better preview with many features
- **Code Spell Checker**: Catches spelling errors in your content
- **Markdown Lint**: Ensures consistent Markdown formatting
- **Markdown Emoji**: Adds emoji support to your Markdown

## Tips and Best Practices

1. **Pull Before Editing**: If you've made changes on another device or if collaborators have pushed changes, always pull first:
   - In VSCode: Click the "..." in Source Control and select "Pull"

2. **Commit Frequently**: Make small, focused commits with clear messages

3. **Use .gitignore**: We've set up a .gitignore file to exclude Obsidian configuration files. If you need to exclude other files, add them to this file.

4. **Resolve Conflicts**: If you get merge conflicts, VSCode has good tools to help resolve them

5. **Backup**: While Git provides version control, it's still good practice to maintain separate backups of important content

## Troubleshooting

- **Changes not showing in VSCode**: Try refreshing the explorer panel
- **Can't commit in VSCode**: Make sure you've staged your changes first
- **Push rejected**: Pull first, resolve any conflicts, then push again
