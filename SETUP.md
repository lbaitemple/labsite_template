# Setup Guide

## Initial Setup

1. **Clone or Download** this template

2. **Install Jekyll and Dependencies**
   ```bash
   gem install bundler jekyll
   bundle install
   ```

3. **Configure Your Site**
   
   Edit `_config.yml`:
   - Change `title` to your lab name
   - Update `email` with your contact email
   - Modify `description` with your lab description
   - Set `baseurl` (empty for root, or "/repo-name" for GitHub Pages)
   - Update `url` to your site URL
   - Change `releases_url` for thesis/report downloads

4. **Add Your Content**

### Adding Images

Place images in the appropriate folders:
- `images/team/` - Team member photos (e.g., pi.jpg, student.jpg)
- `images/team/alumni/YEAR/` - Alumni photos organized by graduation year
- `images/slider/` - Homepage slider images (will auto-load all images)
- `images/research/` - Research project images
- `images/news/` - News article images
- `images/logo/` - Lab logo

**Image naming conventions:**
- Team photos: Use lowercase with hyphens (e.g., john-doe.jpg)
- Keep images reasonably sized (< 1MB recommended)

### Adding Team Members

1. Create a new markdown file in `_pages/team/` for current members
2. For alumni, create files in `_pages/team/alumni/YEAR/`
3. Add corresponding photo to `images/team/` or `images/team/alumni/YEAR/`

**Example:** `_pages/team/jane-smith.md`
```yaml
---
layout: member
category: student
title: Jane Smith
image: jane-smith.jpg
role: PhD Student
permalink: /team/jane-smith
social:
    linkedin: https://linkedin.com/in/janesmith
    github: https://github.com/janesmith
education:
  - MS, Computer Science, University, 2020
---

Bio text here.
```

### Adding Research Projects

1. Create markdown files in `_pages/research/`
2. Set `order` field (higher = more recent, shows expanded)
3. Add team members who worked on the project

### Adding Publications

Edit `_data/publications.json` and add entries:
```json
{
  "title": "Paper Title",
  "authors": "Author1, Author2",
  "venue": "Conference/Journal Name",
  "year": 2024,
  "type": "conference",
  "pdf": "https://link-to-pdf.com"
}
```

### Adding News

Edit `_data/news.yml`:
```yaml
- date: MM/DD/YY
  title: "News Title"
  image: "news/image.jpg"  # Optional
  tags:
    - tag1
    - tag2
  content: >
    News content here.
```

## Running Locally

```bash
bundle exec jekyll serve
```

Visit `http://localhost:4000`

## Deployment

### GitHub Pages

1. Push to GitHub repository
2. Go to Settings > Pages
3. Select branch (usually `main` or `master`)
4. Save

Your site will be available at `https://username.github.io/repo-name/`

### Custom Domain

1. Add `CNAME` file with your domain
2. Configure DNS settings with your domain provider

## Customization

### Colors and Styling

Edit `css/main.scss` to customize:
- Colors
- Fonts
- Spacing
- Layout

### Navigation

Edit `_includes/header.html` to modify navigation menu items.

### Footer

Edit `_includes/footer.html` to customize footer content.

## Troubleshooting

**Build errors:**
- Check YAML front matter syntax
- Ensure all required fields are present
- Verify image paths are correct

**Images not showing:**
- Check file paths in markdown files
- Ensure images exist in correct folders
- Verify `baseurl` in `_config.yml`

**Styling issues:**
- Clear browser cache
- Check CSS file paths
- Verify Bootstrap is loading

## Support

For issues or questions:
- Check Jekyll documentation: https://jekyllrb.com/docs/
- Review GitHub Pages docs: https://docs.github.com/en/pages

## License

This template is free to use for academic purposes.
