# Academic Lab Website Template

A clean, modern Jekyll template for academic research lab websites.

[Demo site](https://lbaitemple.github.io/labsite_template/)

## Features

- **Home Page**: Dynamic image slider with lab description
- **Team Page**: Organized by staff, students (PhD/Master/Undergrad), and alumni by graduation year
- **Research Page**: Project showcase with search, category filters, and team member listings
- **Publications Page**: Tabbed view (Conference/Journal/By Year/Search) with automatic numbering
- **News Page**: News feed with optional images and tags
- **Software Page**: Showcase lab software and tools

## Quick Start

1. **Install Dependencies**
   ```bash
   bundle install
   ```

2. **Configure Your Site**
   - Edit `_config.yml` with your lab information
   - Update `baseurl` and `url` for your deployment

3. **Add Content**
   - Team members: `_pages/team/`
   - Research projects: `_pages/research/`
   - Publications: `_data/publications.json`
   - News: `_data/news.yml`
   - Images: `images/` folder

4. **Run Locally**
   ```bash
   bundle exec jekyll serve
   ```
   Visit `http://localhost:4000`

5. **Deploy**
   - Push to GitHub and enable GitHub Pages in repository settings
   - Or deploy to any Jekyll-compatible hosting

## Directory Structure

```
├── _config.yml           # Site configuration
├── _data/               # Data files
│   ├── news.yml         # News items
│   └── publications.json # Publications list
├── _includes/           # Reusable components
├── _layouts/            # Page layouts
├── _pages/              # Site pages
│   ├── home.md
│   ├── team/            # Team member files
│   ├── research/        # Research project files
│   ├── publications.html
│   ├── news.html
│   └── software.md
├── _sass/               # Sass stylesheets
├── css/                 # Main CSS
├── images/              # Images
│   ├── team/            # Team photos
│   ├── research/        # Research images
│   ├── slider/          # Homepage slider images
│   ├── news/            # News images
│   └── logo/            # Lab logo
├── fonts/               # Web fonts
├── js/                  # JavaScript files
└── vendor/              # Third-party libraries
```

## Customization

### Adding Team Members

Create a new file in `_pages/team/` (e.g., `john-doe.md`):

```yaml
---
layout: member
category: student  # staff, student, or past
title: John Doe
image: john-doe.jpg
role: PhD Student  # or "Master Student", "Undergraduate Student", "Alumni"
permalink: /team/john-doe
grad_year: 2025  # For alumni only
social:
    linkedin: https://linkedin.com/in/johndoe
    github: https://github.com/johndoe
education:
  - BS Computer Science, University Name, 2020
---

Bio text here.
```

### Adding Research Projects

Create a new file in `_pages/research/` (e.g., `my-project.md`):

```yaml
---
layout: default
title: "My Research Project"
description: "Brief project description"
permalink: /research/my-project
categories:
  - AI/ML
  - Healthcare
order: 5
year: "2023-Present"
team:
  - name: "John Doe"
    role: "PhD Student"
---

Detailed project description here.
```

### Adding Publications

Edit `_data/publications.json`:

```json
{
  "publications": [
    {
      "title": "Paper Title",
      "authors": "Author1, Author2, Author3",
      "venue": "Conference/Journal Name",
      "year": 2024,
      "type": "conference",
      "pdf": "https://link-to-pdf.com",
      "doi": "10.1234/example"
    }
  ]
}
```

### Adding News

Edit `_data/news.yml`:

```yaml
- date: 01/15/24
  title: "News Title"
  image: "news/image.jpg"  # Optional
  tags:
    - award
    - publication
  content: >
    News content here.
```

## License

This template is open source and available for academic use.

## Support

For issues or questions, please open an issue on GitHub.
