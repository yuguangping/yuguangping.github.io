# Personal Homepage Checklist

This site is based on the AcadHomepage Jekyll template.

## Edit These Files First

- `_config.yml`: site title, description, repository, avatar, email, GitHub, Google Scholar, LinkedIn, ORCID, and location.
- `_pages/about.md`: the homepage content: bio, news, research interests, projects, publications, education, experience, awards, and contact.
- `_data/navigation.yml`: the top navigation links.
- `images/`: replace the default avatar and project images.

## Local Preview

This project needs Ruby and Bundler for local preview.

```powershell
bundle install
bundle exec jekyll serve
```

Then open `http://127.0.0.1:4000`.

Ruby/Bundler are not currently installed on this Windows machine, so GitHub Pages can also build the site after you push it to GitHub.

## Publish on GitHub Pages

1. Create a GitHub repository named `yuguangping.github.io`.
2. Push this folder to that repository.
3. In GitHub, open `Settings -> Pages`.
4. Select deployment from the `main` branch.
5. Your homepage should appear at `https://yuguangping.github.io`.

## Optional Google Scholar Citations

If you want automatic citation stats:

1. Find your Google Scholar ID from a URL like `https://scholar.google.com/citations?user=SCHOLAR_ID`.
2. In the GitHub repository, add a repository secret named `GOOGLE_SCHOLAR_ID`.
3. Enable GitHub Actions for the repository.
4. Set `google_scholar_stats_enabled: true` in `_config.yml`.
5. Set `google_scholar_stats_use_cdn` in `_config.yml` if you want to use the CDN path from the original template.
