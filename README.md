# VisualStudioCode - `vscode-color-customizations`


````md
# VS Code Color Customizations (Settings Snippet)

A small, clean `settings.json` snippet to customize VS Code UI colors (cursor, line numbers, selection, bracket highlights, tabs, status bar) and terminal colors (ANSI palette).

## Files

- **`workbench.colorCustomizations.json** 

## How to use

1. Open VS Code
2. Go to **Settings (JSON)**:
   - `Ctrl + Shift + P` / `Cmd + Shift + P`
   - Search: **Preferences: Open Settings (JSON)**
3. Copy the contents from `settings.jsonc`
4. Paste into your `settings.json`
5. Save and restart VS Code (sometimes required for UI refresh)

## Snippet

> You can paste this whole block into your VS Code `settings.json`.

```jsonc
{
  "workbench.colorCustomizations": {
    // Editor
    "editorCursor.foreground": "#61DAFB",
    "editorLineNumber.foreground": "#858585",
    "editorLineNumber.activeForeground": "#61DAFB",
    "editor.selectionBackground": "#3A3A41",
    "editor.selectionHighlightBackground": "#264F78",

    // Brackets
    "editorBracketHighlight.foreground1": "#FFD700", // gold
    "editorBracketHighlight.foreground2": "#ADFF2F", // green-yellow
    "editorBracketHighlight.foreground3": "#00BFFF", // sky blue
    "editorBracketHighlight.unexpectedBracket.foreground": "#FF6347", // tomato red

    // Status bar
    "statusBar.debuggingBackground": "#D16969",
    "statusBar.noFolderBackground": "#68217A",

    // Tabs
    "tab.activeBorder": "#61DAFB",
    "tab.activeBackground": "#20232A",
    "tab.inactiveBackground": "#1E1E1E",

    // Terminal
    "terminal.background": "#1E1E1E",
    "terminal.foreground": "#D4D4D4",
    "terminalCursor.foreground": "#61DAFB",

    // Terminal ANSI colors
    "terminal.ansiBlack": "#000000",
    "terminal.ansiRed": "#FF5555",
    "terminal.ansiGreen": "#50FA7B",
    "terminal.ansiYellow": "#F1FA8C",
    "terminal.ansiBlue": "#61DAFB",
    "terminal.ansiMagenta": "#FF79C6",
    "terminal.ansiCyan": "#8BE9FD",
    "terminal.ansiWhite": "#F8F8F2",

    "terminal.ansiBrightBlack": "#555555",
    "terminal.ansiBrightRed": "#FF6E6E",
    "terminal.ansiBrightGreen": "#69FF94",
    "terminal.ansiBrightYellow": "#FFFFA5",
    "terminal.ansiBrightBlue": "#6FC1FF",
    "terminal.ansiBrightMagenta": "#FF92DF",
    "terminal.ansiBrightCyan": "#A4FFFF",
    "terminal.ansiBrightWhite": "#FFFFFF"
  },

  "editor.renderWhitespace": "all",
  "editor.renderLineHighlight": "all",
  "editor.guides.indentation": true,

  // Built-in icon theme id:
  "workbench.iconTheme": "vs-seti"
}
````

## Notes

* If you already have other settings in `settings.json`, merge this carefully (don’t duplicate keys).
* If you prefer a different icon theme, replace `"workbench.iconTheme"` with the exact theme id shown in:
  **File → Preferences → Theme → File Icon Theme**.




