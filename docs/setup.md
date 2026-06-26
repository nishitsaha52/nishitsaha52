# GitHub Profile Setup

This folder is designed to become your GitHub profile repository.

## 1. Create the profile repository

Create a public repository named exactly:

```text
nishitsaha52/nishitsaha52
```

GitHub renders the `README.md` from that repository on your profile page.

## 2. Copy these files

Copy everything from:

```text
github-profile/
```

into the root of your `nishitsaha52/nishitsaha52` repository.

Expected structure:

```text
README.md
assets/
.github/workflows/
profile-3d-contrib/
docs/
```

## 3. Enable GitHub Actions

Open the repository on GitHub, then go to:

```text
Settings -> Actions -> General
```

Enable actions if GitHub asks.

## 4. Run the workflows

Go to the `Actions` tab and manually run:

- `Generate contribution snake`
- `Generate 3D contribution profile`
- `Generate profile metrics`

The snake workflow publishes files to the `output` branch.

## 5. Metrics token

The metrics workflow uses `lowlighter/metrics` and expects a secret named:

```text
METRICS_TOKEN
```

Create a fine-grained GitHub token with read-only profile and repository access, then add it under:

```text
Settings -> Secrets and variables -> Actions -> New repository secret
```

If you do not want metrics, delete `.github/workflows/metrics.yml`.

## 6. Personalize optional sections

Before publishing, update these optional areas in `README.md`:

- Blog links
- Public repository links for featured projects
- Any certifications you want to link to credential URLs
- Any additional social links

## 7. Final check

After pushing, open:

```text
https://github.com/nishitsaha52
```

Give widgets a few minutes to render. Some external widgets may cache aggressively, so first render can be slow.
