# Publish Steps

This folder is already prepared as a GitHub Pages personal homepage project.

## 1. Edit Personal Information

Before publishing, update:

- `_config.yml`: name, bio, email, location, avatar, GitHub, Scholar, LinkedIn, ORCID.
- `_pages/about.md`: biography, news, research interests, projects, publications, education, experience, awards, contact.
- `images/`: replace avatar and project images.

## 2. Create GitHub Repository

Create a public repository named:

```text
yuguangping.github.io
```

For a GitHub user site, the repository name must match this form.

## 3. Push This Folder

Run these commands in PowerShell:

```powershell
cd C:\Users\yuguangping\yuguangping.github.io
git add .
git commit -m "Initialize personal homepage"
git remote add origin https://github.com/yuguangping/yuguangping.github.io.git
git push -u origin main
```

If `origin` already exists, use:

```powershell
git remote set-url origin https://github.com/yuguangping/yuguangping.github.io.git
git push -u origin main
```

## 4. Enable GitHub Pages

Open the repository on GitHub:

```text
Settings -> Pages
```

Use:

```text
Source: Deploy from a branch
Branch: main
Folder: / root
```

After GitHub finishes building, the site should be available at:

```text
https://yuguangping.github.io
```

## 5. Optional Local Preview

Local preview requires Ruby and Bundler:

```powershell
bundle install
bundle exec jekyll serve
```

Then open:

```text
http://127.0.0.1:4000
```
