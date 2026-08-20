# GitHub Profile README — Setup

## Files

- `README.md` — replace the existing profile README with this.
- `assets/profile.png` — your supplied profile image.
- `assets/hero.svg` — custom premium hero with animated green availability indicator.
- `.github/workflows/contribution-snake.yml` — automatically regenerates the contribution animation.

## Install

Copy the files into the root of `mashood17/mashood17`:

```text
mashood17/
├── README.md
├── assets/
│   ├── profile.png
│   └── hero.svg
└── .github/
    └── workflows/
        └── contribution-snake.yml
```

Commit everything to `main`.

## First run

The contribution snake SVG does not exist until GitHub Actions runs once.

After the first workflow run, these files will be created automatically:

```text
assets/github-contribution-snake.svg
assets/github-contribution-snake-dark.svg
```

The workflow runs:
- on every push to `main`
- once every day
- manually from the Actions tab

No contribution counts are hard-coded in the README.

## Important

The dynamic GitHub stats cards use external services. The core branding, hero, profile image and contribution animation are local repository assets, so the most important visual elements do not depend on a third-party banner service.

If GitHub Actions is disabled for the profile repository, enable Actions and run **Update contribution animation** manually once.
