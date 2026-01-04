# Practice! Documentation

This is the documentation site for Practice!, built with Jekyll and hosted on GitHub Pages.

## Setup

1. Install Ruby and Bundler
2. Run `bundle install` to install dependencies
3. Run `bundle exec jekyll serve` to preview locally
4. Visit `http://localhost:4000/practice/` to view the site

## Deployment

This site is configured for GitHub Pages. Simply push to the `main` branch and GitHub Pages will automatically build and deploy the site.

## Adding Screenshots

Place screenshots in the `assets/images/` directory and reference them in markdown files:

```markdown
![App Icon Example]({{ '/assets/images/app-icon.png' | relative_url }})
```

## Documentation Structure

- `index.md` - Getting started guide
- `practice-sessions.md` - Practice session documentation
- `spaced-repetition.md` - Spaced repetition system
- `goals.md` - Practice goals
- `exercises.md` - Exercises
- `plans.md` - Practice plans
- `organizing.md` - Organizing tunes
- `data-management.md` - Data import/export
- `settings.md` - App settings

## Updating the Base URL

When deploying to a custom domain, update `baseurl` in `_config.yml`:

```yaml
baseurl: "/practice"  # Change this to match your domain structure
```

Also update the URL in the app's `HelpConfig.swift` file to match.

