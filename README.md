# Git Master Sync

`git-master-sync` is a Bash script that automates the maintenance of your Git branches.

## ✨ Features

- Fetches and updates the `master` branch from the remote repository.
- Updates all active local branches by merging the latest changes from `master`.
- Automatically deletes local branches that:
  - no longer exist on the remote;
  - have already been merged into `master`.
- Includes a `--dry-run` mode to preview actions without making any changes.

## 📥 Installation

1. Clone this repository into a folder of your choice (example: `~/tools/`):
   ```bash
   git clone https://github.com/your-username/git-master-sync.git ~/tools/git-master-sync
   ```

2. Add the script directory to your environment variables so it can be used everywhere:
   ```bash
   echo 'export PATH="$HOME/tools/git-master-sync:$PATH"' >> ~/.bashrc
   source ~/.bashrc
   ```

3. Make the script executable:
   ```bash
   chmod +x ~/tools/git-master-sync/git-master-sync
   ```

Now you can run `git-master-sync` from any directory.

## ▶️ Usage

Run with real updates and branch deletions:
```bash
git-master-sync
```

Preview actions without making changes:
```bash
git-master-sync --dry-run
```

## ⚙️ Requirements

- Git installed and accessible from your shell.
- Bash environment (Linux, macOS, or Windows with Git Bash).
