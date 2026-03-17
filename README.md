# Peace Equalizer APO Extension - Source Sync

This repository is an automated mirror that synchronizes the source code of the [Peace Equalizer APO extension](https://sourceforge.net/projects/peace-equalizer-apo-extension/) from SourceForge to GitHub.

## How it works

A GitHub Action runs daily to:
1. Check the MD5 hash of the latest source code on SourceForge.
2. If a new version is detected, it downloads and extracts it into the `upstream/` directory.
3. It creates a new branch and opens a Pull Request with the updated source code.

## Setup Requirements

For the automation to function correctly, you must enable Pull Request permissions for GitHub Actions:

1.  Go to your repository **Settings**.
2.  Navigate to **Actions** > **General**.
3.  Under **Workflow permissions**, ensure **Allow GitHub Actions to create and approve pull requests** is checked.
4.  Click **Save**.

## License

This project is licensed under the GNU General Public License v2.0 (GPL-2.0).
