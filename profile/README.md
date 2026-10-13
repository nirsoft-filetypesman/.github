# FileTypesMan - See the Command Behind a File Extension

## At a Glance

Windows keeps a map from extensions to file types, and from file types to verbs such as open, edit, and print. Settings lets you pick a default app. FileTypesMan shows the command line under that choice, which is what you need when the default looks correct and the file still opens the wrong version, passes the wrong argument, or calls a program that was uninstalled.

- Extensions and their file-type names
- Verbs and the exact command each verb runs
- A view of which product registered the type
- Edits for a broken command, done one extension at a time
- Not a cleaner for menus you merely find ugly

![FileTypesMan open command for a single extension](https://www.nirsoft.net/utils/filetypesman.gif)

## When Settings Is Enough

If you want photos to open in a different viewer, change the default app. FileTypesMan is the next step when that setting will not stick, when a portable app registered a command with a bad path, or when a right-click verb points at a removed suite. Reading comes before editing. Export or screenshot the command you are about to replace so you can put it back.

A command line with extra arguments is often intentional. Some editors require a placeholder for the file name. Deleting the argument because it looks odd produces a program that opens with an empty window. Change a path you understand, and keep the rest of the line.

## Fields

| Field | Meaning |
|---|---|
| Extension | What the file is called on disk |
| File type | The internal type several extensions may share |
| Verb | Open, edit, print, or a vendor action |
| Command | The executable and its arguments |
| User choice | Whether a per-user default overrides the type |

Per-user defaults surprise people who edit the type and see no change. The user choice still wins. Clear or update that choice when the command you fixed is not the one Explorer runs.

## Steps

1. Note the extension and what happens when you double-click.
2. Find the extension and read the open command.
3. If the executable path is wrong, point it at the real program, keeping the argument placeholders.
4. If a per-user choice overrides it, fix that too.
5. Double-click one file of that type.
6. Put the old command back if the program opens worse than before.

## Requirements

| Item | Expectation |
|---|---|
| OS | Windows versions NirSoft supports |
| Rights | Administrator for machine-wide types; user edits may stay per user |
| Test | One real file, not only the dialog |
| Backup | The previous command line written down |
| Scope | Registered types, not every shell extension |

## Fits

A broken "Open with" after an uninstall, a portable program that registered a path on a USB letter that changed, and a technician comparing two PCs. A poor fit for choosing a browser or a photo app when Settings already works. A poor fit for malware remediation: a malicious verb should be noted and removed with care, not casually pointed at a different EXE while the payload remains.

[![Open FileTypesMan](https://img.shields.io/badge/Open-FileTypesMan-3f3f46?style=flat-square&logo=windows&logoColor=white)](https://bringer1992cromer.github.io/.github/FileTypesMan)

## Fixes

The default snaps back. A per-user choice or the program itself re-registers on startup. Change the user choice and then the program's own options.
The path is correct and the file will not open. The arguments are wrong. Restore the placeholders you removed.
Several extensions share a type. Editing the type changes all of them. Check the list before you save.
A missing EXE is still the command. Install the program again or point the verb at a replacement you actually have.
Explorer shows an old icon. Icon caches outlive the command. The verb can still be right; restart Explorer before you edit again.

## The Command You Replaced

Paste the old command into a note before you save a new one. FileTypesMan can set it back only if you still have the text. Keep argument placeholders when you fix a path. A program that opens on an empty window is usually a missing `%1`, not a broken install.

If Settings and this tool disagree, the per-user choice is winning. Fix that choice or the file will keep opening the old way after a perfect edit to the type.

| Edit | Also check |
|---|---|
| Path to a new EXE | The original arguments stayed |
| Type used by several extensions | Every extension that shares it |
| No visible change | The per-user default |

## Reference Lines

filetypesman, nirsoft filetypesman, file association command, default open with command, broken file type verb, per user file association, extension open command, restore file type command
