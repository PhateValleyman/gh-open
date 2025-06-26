# gh-open

`gh-open` is a terminal utility written in Bash that opens the current GitHub/GitLab/Bitbucket page (repository, file, or directory) in your default browser from the command line.

## Features

- 🧠 Smart remote detection (tracking → origin → fallback)
- 🔀 SSH-to-HTTPS URL conversion
- 🌲 Directory vs 📄 File context-aware link building
- 🌿 Branch and commit-aware navigation
- 🧪 Dry-run support
- 📁 Works from outside the Git repo when path points inside one

## Usage

```bash
gh open [options] [<path>]
```

### Options:

- `-r <remote>` — use specific remote
- `-b <branch>` — override branch or commit
- `-n` — dry-run (only print URL)
- `-v` — print version
- `-h` — show help

### Examples:

```bash
gh open                 # opens current repo path
gh open README.md       # opens file in web
gh open docs/           # opens docs dir
gh open -n src/file.c   # prints the URL without opening
```

## Compatibility

- ✅ Termux (Android)
- ✅ Linux (xdg-open)
- ✅ macOS (with `open`)
- ❓ Windows (not tested)

## Author

**PhateValleyman**  
Jonas.Ned@outlook.com

