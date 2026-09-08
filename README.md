# Practice! Documentation

This is the documentation site for Practice!, built with Jekyll and hosted on GitHub Pages.

## Setup

1. Install Ruby and Bundler
2. Run `bundle install` to install dependencies
3. Run `bundle exec jekyll serve` to preview locally
4. Visit `http://localhost:4000/practice/` to view the site

## Deployment

This site is configured for GitHub Pages. Simply push to the `main` branch and GitHub Pages will automatically build and deploy the site.

## No screenshots

The prose pages carry no screenshots, deliberately. Every one they had was
years out of date and showed controls that had moved or been renamed — worse
than no picture, because a stale image sitting beside correct text reads as an
instruction. Keeping them current means re-shooting the set every time a screen
changes, which nobody was ever going to do.

Where a screen genuinely needs showing, film it: the how-to videos under
`how-to/` are regenerated from the storyboards in the app repo and go out of
date gracefully. Don't reintroduce stills here.

## Documentation Structure

- `index.md` - Getting started guide
- `practice-sessions.md` - Practice session documentation
- `spaced-repetition.md` - Comfort Levels and the Repertoire
- `goals.md` - Practice goals
- `exercises.md` - Exercises
- `organizing.md` - Organizing tunes
- `data-management.md` - Data import/export
- `settings.md` - App settings
- `how-to/` - The how-to videos. **Generated** — do not edit by hand. The
  storyboards live in the app repo at `docs/videos/`; rebuild with
  `scripts/build_tour_docs.py --out ../FolkTunesApp-docs/how-to` from there.

## Updating the Base URL

When deploying to a custom domain, update `baseurl` in `_config.yml`:

```yaml
baseurl: "/practice"  # Change this to match your domain structure
```

Also update the URL in the app's `HelpConfig.swift` file to match.

