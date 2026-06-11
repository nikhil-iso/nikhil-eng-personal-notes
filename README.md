# Nikhil Engineering Notes

This repository is a personal archive for engineering notes, experiment logs, Jupyter notebooks, reference material, and supporting images. It is intended for record retention first: keep the original thinking, assumptions, calculations, plots, and observations close to the work.

## Repository Layout

```text
.
├── notebooks/      # Jupyter notebooks and engineering logbooks
├── images/         # Photos, diagrams, plots, screenshots, and other media
├── exports/        # Optional rendered PDFs, HTML exports, or shared snapshots
└── references/     # Datasheets, papers, links, and supporting source material
```

Existing notebooks can stay at the root temporarily, but new notes should go in `notebooks/` so the archive stays easy to scan.

## Naming Notes

Use descriptive, date-prefixed names when the note is tied to a specific session or experiment:

```text
YYYY-MM-DD_topic_or_project_note.ipynb
YYYY-MM-DD_topic_or_project_log.md
```

Examples:

```text
2026-06-11_rocketry_motor_sizing.ipynb
2026-06-11_flight-test-observations.md
```

## Notebook Practices

- Keep enough context in each notebook to understand the work later: goal, assumptions, inputs, outputs, and next steps.
- Prefer relative paths for images and data so notebooks remain portable inside the repo.
- Commit notebooks after meaningful checkpoints, not only when they are polished.
- Clear large transient outputs when they are not useful for the long-term record.
- Put generated exports in `exports/` when a stable PDF or HTML snapshot is useful.

## Local Setup

Create and activate a local Python environment if you want to run notebooks from this repo:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install jupyterlab ipykernel numpy pandas matplotlib scipy
python -m ipykernel install --user --name nikhil-eng-notes --display-name "Nikhil Engineering Notes"
jupyter lab
```

If a notebook needs specialized packages, install them in the virtual environment and record the package names in the notebook or a project-specific note.

## Retention Guidelines

- Keep raw observations and reasoning, even when later analysis changes.
- Add links or citations for external references when they influenced a decision.
- Store important images or screenshots in `images/` instead of relying only on external links.
- Use `references/` for durable copies of datasheets, papers, and design notes when license terms allow it.

## Git Hygiene

This repo ignores local virtual environments, Jupyter checkpoints, caches, temporary files, and OS/editor noise. Large binaries should be committed intentionally only when they are part of the retained engineering record.
