# git-master-sync

`git-master-sync` is a Bash script that automates the maintenance of your Git branches.

## Features

- Fetches and updates the `master` branch from the remote repository.
- Updates all active local branches by merging the latest changes from `master`.
- Automatically deletes local branches that:
  - no longer exist on the remote;
  - have already been merged into `master`.
- Includes a `--dry-run` mode to preview actions without making any changes.

## Installation

1. Save the script as `git-master-sync` in a directory included in your `$PATH` (e.g., `~/.local/bin/`).
2. Make it executable:
   ```bash
   chmod +x ~/.local/bin/git-master-sync
