# gh-open

`gh-open` is a terminal utility written in Bash that opens the current GitHub/GitLab/Bitbucket page (repository, file, or subdirectory) in your default browser from the command line.

## Features

- 🧠 Smart remote detection (tracking → origin → first)
- 🔀 SSH-to-HTTPS URL conversion
- 🌲 Directory vs 📄 File context-aware link building
- 🌿 Branch and commit-aware navigation
- 🧪 Dry-run support (`-n`)
- 🔄 Opens current directory when no path is given, preserving subdirectory context

## Usage

```bash
gh-open [options] [<path>]
```

### Options:

- `-r <remote>` — use specific remote (default `origin`)
- `-b <branch>` — override branch or commit (default current branch)
- `-n` — dry-run (prints the URL only)
- `-v` — print version (`v1.0`)
- `-h` — show help message

### Examples

```bash
gh-open               # opens web view of current directory
gh-open README.md     # opens specific file
gh-open src/          # opens subdirectory tree view
gh-open -n docs/      # prints URL without opening
gh-open -b develop    # open current directory on 'develop' branch
```

## Installation

Place the `gh-open` script in your PATH, e.g.:

```bash
mv gh-open /usr/local/bin/gh-open
chmod +x /usr/local/bin/gh-open
```

## Author

**PhateValleyman**  
Jonas.Ned@outlook.com
